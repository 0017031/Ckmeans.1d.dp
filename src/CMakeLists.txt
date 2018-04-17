cmake_minimum_required(VERSION 2.8)

add_library(ckmeans_1d_dp)

target_sources(ckmeans_1d_dp PRIVATE
        Ckmeans.1d.dp.cpp
        Ckmeans.1d.dp_main.cpp
        dynamic_prog.cpp
        fill_log_linear.cpp
        fill_quadratic.cpp
        fill_SMAWK.cpp
        select_levels.cpp
        weighted_select_levels.cpp
        within_cluster.h)

target_sources(ckmeans_1d_dp PUBLIC
        Ckmeans.1d.dp.h)

target_include_directories(ckmeans_1d_dp PUBLIC
        C:/Users/baic/Downloads/apps/R/R-3.4.4/include)