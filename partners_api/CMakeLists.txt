project(partners_api)

include_directories(${OMIM_ROOT}/3party/jansson/src)

set(
  SRC
  ads_base.cpp
  ads_base.hpp
  ads_engine.cpp
  ads_engine.hpp
  banner.hpp
  booking_api.cpp
  booking_api.hpp
  booking_availability_params.cpp
  booking_availability_params.hpp
  booking_block_params.cpp
  booking_block_params.hpp
  booking_params_base.hpp
  facebook_ads.cpp
  facebook_ads.hpp
  google_ads.cpp
  google_ads.hpp
  locals_api.cpp
  locals_api.hpp
  maxim_api.cpp
  maxim_api.hpp
  megafon_countries.cpp
  megafon_countries.hpp
  mopub_ads.cpp
  mopub_ads.hpp
  opentable_api.cpp
  opentable_api.hpp
  partners.cpp
  partners.hpp
  rb_ads.cpp
  rb_ads.hpp
  taxi_base.cpp
  taxi_base.hpp
  taxi_engine.cpp
  taxi_engine.hpp
  taxi_places.cpp
  taxi_places.hpp
  taxi_places_loader.cpp
  taxi_places_loader.hpp
  taxi_provider.hpp
  uber_api.cpp
  uber_api.hpp
  utils.cpp
  utils.hpp
  viator_api.cpp
  viator_api.hpp
  yandex_api.cpp
  yandex_api.hpp
)

omim_add_library(${PROJECT_NAME} ${SRC})

omim_add_test_subdirectory(partners_api_tests)
