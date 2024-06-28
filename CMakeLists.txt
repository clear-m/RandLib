# Generated from RandLib.pro.

cmake_minimum_required(VERSION 3.16)
project(RandLib VERSION 1.0 LANGUAGES CXX)

set(CMAKE_INCLUDE_CURRENT_DIR ON)

set(CMAKE_AUTOMOC ON)

if(NOT DEFINED INSTALL_EXAMPLESDIR)
    set(INSTALL_EXAMPLESDIR "examples")
endif()

set(INSTALL_EXAMPLEDIR "${INSTALL_EXAMPLESDIR}")

# find_package(QT NAMES Qt5 Qt6 REQUIRED COMPONENTS Core)
# find_package(Qt${QT_VERSION_MAJOR} REQUIRED COMPONENTS Gui)

add_library(RandLib STATIC
    RandLib.h
    RandLib_global.h
    distributions/Distributions.h
    distributions/ProbabilityDistribution.cpp distributions/ProbabilityDistribution.h
    distributions/bivariate/BivariateDistribution.cpp distributions/bivariate/BivariateDistribution.h
    distributions/bivariate/BivariateNormalRand.cpp distributions/bivariate/BivariateNormalRand.h
    distributions/bivariate/ContinuousBivariateDistribution.cpp distributions/bivariate/ContinuousBivariateDistribution.h
    distributions/bivariate/DiscreteBivariateDistribution.cpp distributions/bivariate/DiscreteBivariateDistribution.h
    distributions/bivariate/NormalInverseGammaRand.cpp distributions/bivariate/NormalInverseGammaRand.h
    distributions/bivariate/TrinomialRand.cpp distributions/bivariate/TrinomialRand.h
    distributions/univariate/BasicRandGenerator.cpp distributions/univariate/BasicRandGenerator.h
    distributions/univariate/ExponentialFamily.cpp distributions/univariate/ExponentialFamily.h
    distributions/univariate/UnivariateDistribution.cpp distributions/univariate/UnivariateDistribution.h
    distributions/univariate/continuous/BetaPrimeRand.cpp distributions/univariate/continuous/BetaPrimeRand.h
    distributions/univariate/continuous/BetaRand.cpp distributions/univariate/continuous/BetaRand.h
    distributions/univariate/continuous/CauchyRand.cpp distributions/univariate/continuous/CauchyRand.h
    distributions/univariate/continuous/ContinuousDistribution.cpp distributions/univariate/continuous/ContinuousDistribution.h
    distributions/univariate/continuous/DegenerateRand.cpp distributions/univariate/continuous/DegenerateRand.h
    distributions/univariate/continuous/ExponentialRand.cpp distributions/univariate/continuous/ExponentialRand.h
    distributions/univariate/continuous/ExponentiallyModifiedGaussianRand.cpp distributions/univariate/continuous/ExponentiallyModifiedGaussianRand.h
    distributions/univariate/continuous/FisherFRand.cpp distributions/univariate/continuous/FisherFRand.h
    distributions/univariate/continuous/FrechetRand.cpp distributions/univariate/continuous/FrechetRand.h
    distributions/univariate/continuous/GammaRand.cpp distributions/univariate/continuous/GammaRand.h
    distributions/univariate/continuous/GeometricStableRand.cpp distributions/univariate/continuous/GeometricStableRand.h
    distributions/univariate/continuous/GumbelRand.cpp distributions/univariate/continuous/GumbelRand.h
    distributions/univariate/continuous/InverseGammaRand.cpp distributions/univariate/continuous/InverseGammaRand.h
    distributions/univariate/continuous/InverseGaussianRand.cpp distributions/univariate/continuous/InverseGaussianRand.h
    distributions/univariate/continuous/IrwinHallRand.cpp distributions/univariate/continuous/IrwinHallRand.h
    distributions/univariate/continuous/KolmogorovSmirnovRand.cpp distributions/univariate/continuous/KolmogorovSmirnovRand.h
    distributions/univariate/continuous/LaplaceRand.cpp distributions/univariate/continuous/LaplaceRand.h
    distributions/univariate/continuous/LevyRand.cpp distributions/univariate/continuous/LevyRand.h
    distributions/univariate/continuous/LogNormalRand.cpp distributions/univariate/continuous/LogNormalRand.h
    distributions/univariate/continuous/LogisticRand.cpp distributions/univariate/continuous/LogisticRand.h
    distributions/univariate/continuous/MarchenkoPasturRand.cpp distributions/univariate/continuous/MarchenkoPasturRand.h
    distributions/univariate/continuous/NakagamiRand.cpp distributions/univariate/continuous/NakagamiRand.h
    distributions/univariate/continuous/NoncentralChiSquaredRand.cpp distributions/univariate/continuous/NoncentralChiSquaredRand.h
    distributions/univariate/continuous/NormalRand.cpp distributions/univariate/continuous/NormalRand.h
    distributions/univariate/continuous/ParetoRand.cpp distributions/univariate/continuous/ParetoRand.h
    distributions/univariate/continuous/PlanckRand.cpp distributions/univariate/continuous/PlanckRand.h
    distributions/univariate/continuous/RaisedCosineRand.cpp distributions/univariate/continuous/RaisedCosineRand.h
    distributions/univariate/continuous/SechRand.cpp distributions/univariate/continuous/SechRand.h
    distributions/univariate/continuous/StableRand.cpp distributions/univariate/continuous/StableRand.h
    distributions/univariate/continuous/StudentTRand.cpp distributions/univariate/continuous/StudentTRand.h
    distributions/univariate/continuous/TriangularRand.cpp distributions/univariate/continuous/TriangularRand.h
    distributions/univariate/continuous/UniformRand.cpp distributions/univariate/continuous/UniformRand.h
    distributions/univariate/continuous/WeibullRand.cpp distributions/univariate/continuous/WeibullRand.h
    distributions/univariate/continuous/WignerSemicircleRand.cpp distributions/univariate/continuous/WignerSemicircleRand.h
    distributions/univariate/continuous/circular/CircularDistribution.cpp distributions/univariate/continuous/circular/CircularDistribution.h
    distributions/univariate/continuous/circular/VonMisesRand.cpp distributions/univariate/continuous/circular/VonMisesRand.h
    distributions/univariate/continuous/circular/WrappedExponentialRand.cpp distributions/univariate/continuous/circular/WrappedExponentialRand.h
    distributions/univariate/discrete/BernoulliRand.cpp distributions/univariate/discrete/BernoulliRand.h
    distributions/univariate/discrete/BetaBinomialRand.cpp distributions/univariate/discrete/BetaBinomialRand.h
    distributions/univariate/discrete/BinomialRand.cpp distributions/univariate/discrete/BinomialRand.h
    distributions/univariate/discrete/CategoricalRand.cpp distributions/univariate/discrete/CategoricalRand.h
    distributions/univariate/discrete/DiscreteDistribution.cpp distributions/univariate/discrete/DiscreteDistribution.h
    distributions/univariate/discrete/GeometricRand.cpp distributions/univariate/discrete/GeometricRand.h
    distributions/univariate/discrete/HyperGeometricRand.cpp distributions/univariate/discrete/HyperGeometricRand.h
    distributions/univariate/discrete/LogarithmicRand.cpp distributions/univariate/discrete/LogarithmicRand.h
    distributions/univariate/discrete/NegativeBinomialRand.cpp distributions/univariate/discrete/NegativeBinomialRand.h
    distributions/univariate/discrete/NegativeHyperGeometricRand.cpp distributions/univariate/discrete/NegativeHyperGeometricRand.h
    distributions/univariate/discrete/PoissonRand.cpp distributions/univariate/discrete/PoissonRand.h
    distributions/univariate/discrete/RademacherRand.cpp distributions/univariate/discrete/RademacherRand.h
    distributions/univariate/discrete/SkellamRand.cpp distributions/univariate/discrete/SkellamRand.h
    distributions/univariate/discrete/UniformDiscreteRand.cpp distributions/univariate/discrete/UniformDiscreteRand.h
    distributions/univariate/discrete/YuleRand.cpp distributions/univariate/discrete/YuleRand.h
    distributions/univariate/discrete/ZetaRand.cpp distributions/univariate/discrete/ZetaRand.h
    distributions/univariate/discrete/ZipfRand.cpp distributions/univariate/discrete/ZipfRand.h
    distributions/univariate/singular/CantorRand.cpp distributions/univariate/singular/CantorRand.h
    distributions/univariate/singular/SingularDistribution.cpp distributions/univariate/singular/SingularDistribution.h
    math/BetaMath.cpp math/BetaMath.h
    math/Constants.h
    math/GammaMath.cpp math/GammaMath.h
    math/NumericMath.cpp math/NumericMath.h
    math/RandMath.cpp math/RandMath.h
)

set_target_properties(RandLib
    PROPERTIES
    CXX_STANDARD 23
    CXX_EXTENSIONS off
)
# TODOs: port these
# target_compile_definitions(RandLib PUBLIC
#     RANDLIB_LIBRARY
# )

# target_link_libraries(RandLib PUBLIC
#     Qt::Core
#     Qt::Gui
# )

# target_compile_options(RandLib
#     -Wall
#     -Weffc++
#     -Werror
#     -Wextra
#     -Wnon-virtual-dtor
#     -Wshadow
#     -pedantic
#     -std=c++17
# )

install(TARGETS RandLib
    RUNTIME DESTINATION "${INSTALL_EXAMPLEDIR}"
    BUNDLE DESTINATION "${INSTALL_EXAMPLEDIR}"
    LIBRARY DESTINATION "${INSTALL_EXAMPLEDIR}"
)
