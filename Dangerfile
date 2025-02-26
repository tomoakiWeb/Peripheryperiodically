periphery.binary_path = ENV['PERIPHERY_PATH']
# すべてのファイルに対して警告を表示
periphery.scan_all_files = true

# 警告をエラーとして扱う
periphery.warning_as_error = true

# PRの変更差分に対して未使用コードを検出
periphery.scan(
  project: "Peripheryperiodically.xcodeproj",
  schemes: ["Peripheryperiodically"],
  clean_build: true,
  build_args: "-sdk iphonesimulator"
) do |violation|
  violation.message = "Pay attention please! #{violation.message}"
end