# `hp_upload_cert`

`hp_upload_cert` is a script to automatically update printer certificate when
it gets renewed from Let's Encrypt or similar authority.

## Installation

Setup a cron job:

	# update printer certificate
	32 *    * * *   root    /etc/letsencrypt/hp-upload-cert/hp_upload_cert "printer.example.com"

It will periodically check Let's Encrypt's certificate storage and when a new
certificate appears it will upload it into the printer if online.


## License

Copyright (c) 2017  Josef Kufner <josef@kufner.cz>

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

    http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.


