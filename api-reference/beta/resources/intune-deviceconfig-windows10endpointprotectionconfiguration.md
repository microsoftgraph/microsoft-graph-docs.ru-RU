---
title: Тип ресурса windows10EndpointProtectionConfiguration
description: В этой статье описаны объявляемые методы, свойства и связи, которые предоставляются ресурсом Windows10EndpointProtectionConfiguration.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: da552b162a8c13d61195a2d90662400bf2526de4
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42786721"
---
# <a name="windows10endpointprotectionconfiguration-resource-type"></a>Тип ресурса windows10EndpointProtectionConfiguration

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

В этой статье описаны объявляемые методы, свойства и связи, которые предоставляются ресурсом Windows10EndpointProtectionConfiguration.


Наследуется от [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Перечисление объектов windows10EndpointProtectionConfiguration](../api/intune-deviceconfig-windows10endpointprotectionconfiguration-list.md)|Коллекция [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md)|Перечисление свойств и связей объектов [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md).|
|[Получение объекта windows10EndpointProtectionConfiguration](../api/intune-deviceconfig-windows10endpointprotectionconfiguration-get.md)|[windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md)|Чтение свойств и связей объекта [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md).|
|[Создание объекта windows10EndpointProtectionConfiguration](../api/intune-deviceconfig-windows10endpointprotectionconfiguration-create.md)|[windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md)|Создание объекта [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md).|
|[Удаление объекта windows10EndpointProtectionConfiguration](../api/intune-deviceconfig-windows10endpointprotectionconfiguration-delete.md)|Нет|Удаление объекта [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md).|
|[Обновление объекта windows10EndpointProtectionConfiguration](../api/intune-deviceconfig-windows10endpointprotectionconfiguration-update.md)|[windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md)|Обновление свойств объекта [windows10EndpointProtectionConfiguration](../resources/intune-deviceconfig-windows10endpointprotectionconfiguration.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|roleScopeTagIds|Коллекция String|Список тегов областей для этого экземпляра сущности. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|суппортсскопетагс|Логический|Указывает, поддерживает ли базовая конфигурация устройства назначение тегов области. Назначение свойства Скопетагс не разрешено, если это значение равно false, а сущности не будут отображаться для пользователей с ограниченной областью действия. Это происходит для устаревших политик, созданных в Silverlight, и может быть разрешено путем удаления и повторного создания политики на портале Azure. Это свойство доступно только для чтения. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceManagementApplicabilityRuleOsEdition|[deviceManagementApplicabilityRuleOsEdition](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|Применимость выпусков ОС для этой политики. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceManagementApplicabilityRuleOsVersion|[deviceManagementApplicabilityRuleOsVersion](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|Правило применимости версии ОС для этой политики. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceManagementApplicabilityRuleDeviceMode|[deviceManagementApplicabilityRuleDeviceMode](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|Правило применимости режима устройства для этой политики. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|createdDateTime|DateTimeOffset|Дата и время создания объекта. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|description|String|Указанное администратором описание конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|displayName|Строка|Указанное администратором имя конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|version|Int32|Версия конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|дмагуарддевицеенумератионполици|[дмагуарддевицеенумератионполицитипе](../resources/intune-deviceconfig-dmaguarddeviceenumerationpolicytype.md)|Эта политика предназначена для обеспечения дополнительной защиты от внешних устройств с поддержкой прямого доступа к памяти. Он обеспечивает более полный контроль над перечислением устройств с поддержкой внешних устройств с поддержкой прямого доступа к памяти, несовместимых с пересопоставлением и изоляцией памяти устройств и изолированной средой. Эта политика вступает в силу только тогда, когда система защиты DMA поддерживается и включена встроенным встроенным по. Защита от DMA ядра — это компонент платформы, который невозможно контролировать с помощью политики или конечным пользователем. Она должна поддерживаться системой на момент производства. Чтобы проверить, поддерживает ли система защиту DMA, проверьте поле Защита ядра DMA на странице Сводка объекта MSINFO32. exe. Возможные значения: `deviceDefault`, `blockAll`, `allowAll`.|
|фиреваллрулес|Коллекция [виндовсфиреваллруле](../resources/intune-deviceconfig-windowsfirewallrule.md)|Настраивает параметры правила брандмауэра. Эта коллекция может содержать не более 150 элементов.|
|усерригхтсакцесскредентиалманажераструстедкаллер|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Это право пользователя используется диспетчером учетных данных во время резервного копирования и восстановления. Сохраненные учетные данные пользователей могут быть скомпрометированы, если эта привилегия передана другим субъектам. Поддерживаются только состояния NotConfigured и Allowed.|
|усерригхтсалловакцессфромнетворк|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Это право пользователя определяет, какие пользователи и группы могут подключаться к компьютеру через сеть. Допустимое состояние — Supported.|
|усерригхтсблоккакцессфромнетворк|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Это право пользователя определяет, каким пользователям и группам запрещается подключаться к компьютеру через сеть. Блок состояния поддерживается.|
|усерригхтсактаспартофсеоператингсистем|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Это право пользователя позволяет процессу олицетворять любого пользователя без проверки подлинности. Таким образом, процесс может получить доступ к тем же локальным ресурсам, что и пользователь. Поддерживаются только состояния NotConfigured и Allowed.|
|усерригхтслокаллогон|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Это право пользователя определяет, какие пользователи могут входить на компьютер. Допустимые состояния NotConfigured, Поддерживаемые |
|усерригхтсденилокаллогон|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Это право пользователя определяет, какие пользователи не могут войти на компьютер. Состояния NotConfigured, блокировки поддерживаются |
|усерригхтсбаккупдата|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Это право пользователя определяет, какие пользователи могут обходить разрешения для файлов, каталогов, реестра и других постоянных объектов при резервном копировании файлов и каталогов. Поддерживаются только состояния NotConfigured и Allowed.|
|усерригхтсчанжесистемтиме|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Это право пользователя определяет, какие пользователи и группы могут изменять время и дату на внутреннем часовом компьютере. Поддерживаются только состояния NotConfigured и Allowed.|
|усерригхтскреатеглобалобжектс|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Этот параметр безопасности определяет, могут ли пользователи создавать глобальные объекты, доступные для всех сеансов. Пользователи, которые могут создавать глобальные объекты, могут повлиять на процессы, выполняемые в сеансах других пользователей, что может привести к сбою приложения или повреждению данных. Поддерживаются только состояния NotConfigured и Allowed.|
|усерригхтскреатепажефиле|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Это право пользователя определяет, какие пользователи и группы могут вызывать внутренний API, чтобы создать и изменить размер файла подкачки. Поддерживаются только состояния NotConfigured и Allowed.|
|усерригхтскреатеперманентшаредобжектс|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Это право пользователя определяет, какие учетные записи могут использоваться процессами для создания объекта каталога с помощью диспетчера объектов. Поддерживаются только состояния NotConfigured и Allowed.|
|усерригхтскреатесимболиклинкс|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Это право пользователя определяет, может ли пользователь создать символическую ссылку с компьютера, на который они входили. Поддерживаются только состояния NotConfigured и Allowed.|
|усерригхтскреатетокен|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Это право пользователя определяет, какие пользователи и группы могут использоваться процессами для создания маркера, который можно использовать для получения доступа к любому локальному ресурсу, когда процесс использует внутренний API для создания маркера доступа. Поддерживаются только состояния NotConfigured и Allowed.|
|усерригхтсдебугпрограмс|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Это право пользователя определяет, какие пользователи могут прикреплять отладчик к любому процессу или ядру. Поддерживаются только состояния NotConfigured и Allowed.|
|усерригхтсремотедесктопсервицеслогон|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Это право пользователя определяет, каким пользователям и группам запрещается вход в систему в качестве клиента служб удаленных рабочих столов. Поддерживаются только состояния NotConfigured и Block|
|усерригхтсделегатион|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Это право пользователя определяет, какие пользователи могут устанавливать параметр "доверять для делегирования" для объекта пользователя или компьютера. Поддерживаются только состояния NotConfigured и Allowed.|
|усерригхтсженератесекуритяудитс|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Это право пользователя определяет, какие учетные записи могут использоваться процессом для добавления записей в журнал безопасности. Журнал безопасности используется для трассировки несанкционированного доступа к системе.  Поддерживаются только состояния NotConfigured и Allowed.|
|усерригхтсимперсонатеклиент|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Назначение этого права пользователю позволяет программам, выполняемым от имени этого пользователя, олицетворять клиента. Требование этого пользователя для такого рода олицетворения запрещает несанкционированному пользователю подключаться к созданной им службе, а затем олицетворять этого клиента, что может повысить уровень разрешений неавторизованного пользователя до Уровни администрирования или системы. Поддерживаются только состояния NotConfigured и Allowed.|
|усерригхтсинкреасесчедулингприорити|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Это право пользователя определяет, какие учетные записи могут использовать процесс с доступом к свойствам Write для другого процесса, чтобы увеличить приоритет выполнения, назначенный другому процессу. Поддерживаются только состояния NotConfigured и Allowed.|
|усерригхтслоадунлоаддриверс|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Это право пользователя определяет, какие пользователи могут динамически загружать и выгружать драйверы устройств или другой код в режиме ядра. Поддерживаются только состояния NotConfigured и Allowed.|
|усерригхтслоккмемори|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Это право пользователя определяет, какие учетные записи могут использовать процесс для хранения данных в физической памяти, что предотвращает их разбиение данных на виртуальную память на диске. Поддерживаются только состояния NotConfigured и Allowed.|
|усерригхтсманажеаудитингандсекуритилогс|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Это право пользователя определяет, какие пользователи могут задавать параметры аудита доступа к объектам для отдельных ресурсов, таких как файлы, объекты Active Directory и разделы реестра. Поддерживаются только состояния NotConfigured и Allowed.|
|усерригхтсманажеволумес|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Это право пользователя определяет, какие пользователи и группы могут выполнять задачи обслуживания для тома, такие как удаленная дефрагментация. Поддерживаются только состояния NotConfigured и Allowed.|
|усерригхтсмодифифирмваринвиронмент|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Это право пользователя определяет, кто может изменять значения в аппаратной среде. Поддерживаются только состояния NotConfigured и Allowed.|
|усерригхтсмодифйобжектлабелс|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Это право пользователя определяет, какие учетные записи пользователей могут изменять метки целостности объектов, таких как файлы, разделы реестра или процессы, принадлежащие другим пользователям. Поддерживаются только состояния NotConfigured и Allowed.|
|усерригхтспрофилесинглепроцесс|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Это право пользователя определяет, какие пользователи могут использовать средства мониторинга производительности для наблюдения за производительностью системных процессов. Поддерживаются только состояния NotConfigured и Allowed.|
|усерригхтсремотешутдовн|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Это право пользователя определяет, каким пользователям разрешено завершать работу компьютера из удаленного расположения в сети. Неправильное использование этого права пользователя может привести к отказу в обслуживании. Поддерживаются только состояния NotConfigured и Allowed.|
|усерригхтсресторедата|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Это право пользователя определяет, какие пользователи могут обходить разрешения для файлов, каталогов, реестра и других постоянных объектов при восстановлении резервных копий файлов и каталогов, и определяет, какие пользователи могут устанавливать любой действительный субъект безопасности в качестве владельца объекта. Поддерживаются только состояния NotConfigured и Allowed.|
|усерригхтстакеовнершип|[deviceManagementUserRightsSetting](../resources/intune-deviceconfig-devicemanagementuserrightssetting.md)|Это право пользователя определяет, какие пользователи могут становиться владельцами любого защищаемого объекта в системе, включая объекты Active Directory, файлы и папки, принтеры, разделы реестра, процессы и потоки. Поддерживаются только состояния NotConfigured и Allowed.|
|ксбокссервицесенаблексбоксгамесаветаск|Логический|Этот параметр определяет, включена ли функция сохранения игры Xbox (1) или отключена (0).|
|ксбокссервицесакцессориманажементсервицестартупмоде|[сервицестарттипе](../resources/intune-deviceconfig-servicestarttype.md)|Этот параметр определяет, является ли тип запуска службы управления принадлежностью автоматическим (2), вручную (3), отключенным (4). По умолчанию: вручную. Возможные значения: `manual`, `automatic`, `disabled`.|
|ксбокссервицесливеаусманажерсервицестартупмоде|[сервицестарттипе](../resources/intune-deviceconfig-servicestarttype.md)|Этот параметр определяет, является ли тип запуска службы диспетчера Live auth автоматическим (2), вручную (3), отключенным (4). По умолчанию: вручную. Возможные значения: `manual`, `automatic`, `disabled`.|
|ксбокссервицесливегамесавесервицестартупмоде|[сервицестарттипе](../resources/intune-deviceconfig-servicestarttype.md)|Этот параметр определяет, является ли тип запуска службы Live Save Service автоматическим (2), вручную (3), отключенным (4). По умолчанию: вручную. Возможные значения: `manual`, `automatic`, `disabled`.|
|ксбокссервицесливенетворкингсервицестартупмоде|[сервицестарттипе](../resources/intune-deviceconfig-servicestarttype.md)|Этот параметр определяет, является ли тип запуска сетевой службы автоматическим (2), вручную (3), отключенным (4). По умолчанию: вручную. Возможные значения: `manual`, `automatic`, `disabled`.|
|локалсекуритйоптионсблоккмикрософтаккаунтс|Логический|Запретить пользователям добавлять новые учетные записи Майкрософт на этот компьютер.|
|локалсекуритйоптионсблоккремотелогонвисбланкпассворд|Логический|Включите локальные учетные записи, не защищенные паролем, для входа в систему из расположений, отличных от физического устройства. Включено по умолчанию|
|локалсекуритйоптионсдисаблеадминистратораккаунт|Логический|Определяет, включена или отключена учетная запись локального администратора.|
|локалсекуритйоптионсадминистратораккаунтнаме|String|Определите имя другой учетной записи, которая будет связана с идентификатором безопасности (SID) учетной записи "Administrator".|
|локалсекуритйоптионсдисаблегуестаккаунт|Логический|Определяет, включена или отключена Гостевая учетная запись.|
|локалсекуритйоптионсгуестаккаунтнаме|String|Определите имя другой учетной записи, которая будет связана с идентификатором безопасности (SID) для учетной записи "гость".|
|локалсекуритйоптионсалловундокквисаусавингтологон|Логический|Запретите отстыковку портативного компьютера без необходимости входа в систему.|
|локалсекуритйоптионсблоккусерсинсталлингпринтердриверс|Логический|Ограничьте установку драйверов принтеров в рамках подключения к общему принтеру только для администраторов.|
|локалсекуритйоптионсблоккремотеоптикалдривеакцесс|Логический|Включение этого параметра позволяет интерактивно вошедший в систему пользователь получать доступ к устройству чтения компакт-дисков.|
|локалсекуритйоптионсформатандежектофремоваблемедиаалловедусер|[локалсекуритйоптионсформатандежектофремоваблемедиаалловедусертипе](../resources/intune-deviceconfig-localsecurityoptionsformatandejectofremovablemediaallowedusertype.md)|Определите, кому разрешено форматировать и извлекать съемные носители NTFS. Возможные значения: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.|
|локалсекуритйоптионсмачинеинактивитилимит|Int32|Определите максимальное количество минут отсутствия активности на экране входа интерактивного рабочего стола, пока не запустится экранная заставка. Допустимые значения — от 0 до 9999|
|локалсекуритйоптионсмачинеинактивитилимитинминутес|Int32|Определите максимальное количество минут отсутствия активности на экране входа интерактивного рабочего стола, пока не запустится экранная заставка. Допустимые значения — от 0 до 9999|
|локалсекуритйоптионсдонотрекуиректрлалтдел|Логический|Требовать нажатия клавиш CTRL + ALT + DEL, прежде чем пользователь сможет войти в систему.|
|локалсекуритйоптионшиделастсигнединусер|Логический|Не отображать имя последнего пользователя, выполнившего вход на это устройство.|
|локалсекуритйоптионшидеусернамеатсигнин|Логический|Не отображать имя пользователя, выполняющего вход на это устройство, после ввода учетных данных и отображения рабочего стола на устройстве.|
|локалсекуритйоптионслогонмессажетитле|String|Задайте заголовок сообщения для пользователей, пытающихся войти в систему.|
|локалсекуритйоптионслогонмессажетекст|String|Задайте текст сообщения для пользователей, пытающихся войти в систему.|
|localSecurityOptionsAllowPKU2UAuthenticationRequests|Логический|Блокировать запросы проверки подлинности PKU2U на этом устройстве для использования сетевых удостоверений.|
|локалсекуритйоптионсалловремотекаллстосекуритяккаунтсманажерхелпербул|Логический|Помощник по пользовательскому интерфейсу Boolean для объекта Локалсекуритйоптионсалловремотекаллстосекуритяккаунтсманажер|
|локалсекуритйоптионсалловремотекаллстосекуритяккаунтсманажер|String|Измените строку языка определения дескрипторов безопасности по умолчанию, чтобы разрешить или запретить пользователям и группам совершать удаленные вызовы в SAM.|
|локалсекуритйоптионсминимумсессионсекуритифорнтлмсспбаседклиентс|[localSecurityOptionsMinimumSessionSecurity](../resources/intune-deviceconfig-localsecurityoptionsminimumsessionsecurity.md)|Этот параметр безопасности позволяет клиенту требовать согласование 128-разрядного шифрования и/или сеанса защиты сеанса NTLMv2. Возможные значения: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.|
|локалсекуритйоптионсминимумсессионсекуритифорнтлмсспбаседсерверс|[localSecurityOptionsMinimumSessionSecurity](../resources/intune-deviceconfig-localsecurityoptionsminimumsessionsecurity.md)|Этот параметр безопасности позволяет серверу требовать согласование 128-разрядного шифрования и/или сеанса защиты сеанса NTLMv2. Возможные значения: `none`, `requireNtmlV2SessionSecurity`, `require128BitEncryption`, `ntlmV2And128BitEncryption`.|
|lanManagerAuthenticationLevel|[lanManagerAuthenticationLevel](../resources/intune-deviceconfig-lanmanagerauthenticationlevel.md)|Этот параметр безопасности определяет, какой протокол проверки подлинности "запрос/ответ" используется для входа в сеть. Возможные значения: `lmAndNltm`, `lmNtlmAndNtlmV2`, `lmAndNtlmOnly`, `lmAndNtlmV2`, `lmNtlmV2AndNotLm`, `lmNtlmV2AndNotLmOrNtm`.|
|ланманажерворкстатиондисаблеинсекурегуестлогонс|Логический|Если этот параметр включен, клиент SMB будет разрешать небезопасные гостевые входы. Если этот параметр не настроен, клиент SMB будет отклонять небезопасные гостевые входы.|
|локалсекуритйоптионсклеарвиртуалмеморипажефиле|Логический|Этот параметр безопасности определяет, будет ли очищаться файл подкачки виртуальной памяти при завершении работы системы.|
|локалсекуритйоптионсалловсистемтобешутдовнвисаусавингтологон|Логический|Этот параметр безопасности определяет, можно ли завершить работу компьютера, не выполняя вход в Windows.|
|локалсекуритйоптионсалловуиакцессаппликатионелеватион|Логический|Разрешить UIAccess Apps запрос на повышение прав без использования безопасного рабочего стола.|
|локалсекуритйоптионсвиртуализефилеандрегистривритефаилурестоперусерлокатионс|Логический|Виртуализация сбоев записи в файл и реестр для отдельных расположений пользователей|
|локалсекуритйоптионсонлелеватесигнедексекутаблес|Логический|Принудительная проверка пути сертификации PKI для указанного исполняемого файла перед тем, как он будет разрешен для запуска.|
|локалсекуритйоптионсадминистраторелеватионпромптбехавиор|[локалсекуритйоптионсадминистраторелеватионпромптбехавиортипе](../resources/intune-deviceconfig-localsecurityoptionsadministratorelevationpromptbehaviortype.md)|Определите поведение запросов на повышение прав для администраторов в режиме одобрения администратором. Возможные значения: `notConfigured`, `elevateWithoutPrompting`, `promptForCredentialsOnTheSecureDesktop`, `promptForConsentOnTheSecureDesktop`, `promptForCredentials`, `promptForConsent`, `promptForConsentForNonWindowsBinaries`.|
|локалсекуритйоптионсстандардусерелеватионпромптбехавиор|[локалсекуритйоптионсстандардусерелеватионпромптбехавиортипе](../resources/intune-deviceconfig-localsecurityoptionsstandarduserelevationpromptbehaviortype.md)|Определите поведение запросов на повышение прав для стандартных пользователей. Возможные значения: `notConfigured`, `automaticallyDenyElevationRequests`, `promptForCredentialsOnTheSecureDesktop`, `promptForCredentials`.|
|локалсекуритйоптионссвитчтосекуредесктопвхенпромптингфорелеватион|Логический|Разрешить всем запросам на повышение прав доступ к рабочему столу интерактивного пользователя, а не к безопасному рабочему столу. Используются параметры политики поведения запросов для администраторов и стандартных пользователей.|
|локалсекуритйоптионсдетектаппликатионинсталлатионсандпромптфорелеватион|Логический|При установке приложений, требующих повышенных привилегий, запрашиваются учетные данные администратора. Включено по умолчанию|
|локалсекуритйоптионсалловуиакцессаппликатионсфорсекурелокатионс|Логический|Разрешить UIAccess Apps запрос на повышение прав без использования безопасного рабочего стола. Включено по умолчанию|
|локалсекуритйоптионсусеадминаппровалмоде|Логический|Определяет, использует ли встроенная учетная запись администратора режим одобрения администратором или выполняет все приложения с правами полного администратора. Включено по умолчанию|
|локалсекуритйоптионсусеадминаппровалмодефорадминистраторс|Логический|Определить, включен ли режим одобрения администратором и все параметры политики контроля учетных записей, по умолчанию включено|
|локалсекуритйоптионсинформатионшовнонлоккскрин|[localSecurityOptionsInformationShownOnLockScreenType](../resources/intune-deviceconfig-localsecurityoptionsinformationshownonlockscreentype.md)|Настройте сведения о пользователе, которые отображаются, когда сеанс заблокирован. Если этот флажок не установлен, отображаются отображаемое имя пользователя, домен и имя пользователя. Возможные значения: `notConfigured`, `userDisplayNameDomainUser`, `userDisplayNameOnly`, `doNotDisplayUser`.|
|локалсекуритйоптионсинформатиондисплайедонлоккскрин|[локалсекуритйоптионсинформатиондисплайедонлоккскринтипе](../resources/intune-deviceconfig-localsecurityoptionsinformationdisplayedonlockscreentype.md)|Настройте сведения о пользователе, которые отображаются, когда сеанс заблокирован. Если этот флажок не установлен, отображаются отображаемое имя пользователя, домен и имя пользователя. Возможные значения: `notConfigured`, `administrators`, `administratorsAndPowerUsers`, `administratorsAndInteractiveUsers`.|
|локалсекуритйоптионсдисаблеклиентдигиталлисигнкоммуникатионсифсерверагрис|Логический|Этот параметр безопасности определяет, будет ли клиент SMB пытаться согласовать подписывание SMB пакетов.|
|локалсекуритйоптионсклиентдигиталлисигнкоммуникатионсалвайс|Логический|Этот параметр безопасности определяет, требуется ли Подписывание пакетов для клиентского SMB-компонента.|
|локалсекуритйоптионсклиентсендуненкриптедпассвордтосирдпартисмбсерверс|Логический|Если этот параметр безопасности включен, перенаправителем SMB (Server Message Block) разрешено отправлять пароли открытым текстом на серверы SMB сторонних производителей, не поддерживающие шифрование паролей во время проверки подлинности.|
|локалсекуритйоптионсдисаблесервердигиталлисигнкоммуникатионсалвайс|Логический|Этот параметр безопасности определяет, требуется ли подписи пакетов для SMB-компонентов сервера.|
|локалсекуритйоптионсдисаблесервердигиталлисигнкоммуникатионсифклиентагрис|Логический|Этот параметр безопасности определяет, будет ли SMB согласовывать подпись SMB Packet с клиентами, которые их запрашивают.|
|локалсекуритйоптионсрестриктанонимаусакцесстонамедпипесандшарес|Логический|По умолчанию этот параметр безопасности запрещает анонимный доступ к ресурсам и каналам к параметрам именованных каналов, к которым возможен анонимный доступ, и к общедоступным ресурсам, к которым возможен анонимный доступ|
|локалсекуритйоптионсдоноталлованонимаусенумератионофсамаккаунтс|Логический|Этот параметр безопасности определяет, какие дополнительные разрешения будут предоставлены анонимным подключениям к компьютеру.|
|локалсекуритйоптионсаллованонимаусенумератионофсамаккаунтсандшарес|Логический|Этот параметр безопасности определяет, разрешено ли анонимным пользователям выполнять определенные действия, например перечислять имена доменных учетных записей и сетевые общие папки.|
|локалсекуритйоптионсдонотстореланманажерхашвалуеоннекстпассвордчанже|Логический|Этот параметр безопасности определяет, будет ли сохраняться значение хэша LAN Manager (LM) для нового пароля при следующем изменении пароля. По умолчанию он не хранится.|
|локалсекуритйоптионссмарткардремовалбехавиор|[localSecurityOptionsSmartCardRemovalBehaviorType](../resources/intune-deviceconfig-localsecurityoptionssmartcardremovalbehaviortype.md);|Этот параметр безопасности определяет, что происходит при удалении смарт-карты пользователя, выполнившего вход в систему, из устройства чтения смарт-карт. Возможные значения: `lockWorkstation`, `noAction`, `forceLogoff`, `disconnectRemoteDesktopSession`.|
|дефендерсекуритицентердисаблеаппбровсеруи|Логический|Используется для отключения отображения области защиты приложений и браузера.|
|дефендерсекуритицентердисаблефамилюи|Логический|Используется для отключения отображения области семьи.|
|дефендерсекуритицентердисаблехеалсуи|Логический|Используется для отключения отображения области производительности и работоспособности устройства.|
|дефендерсекуритицентердисабленетворкуи|Логический|Используется для отключения отображения зоны "брандмауэр" и "Защита сети".|
|дефендерсекуритицентердисаблевирусуи|Логический|Используется для отключения отображения области защиты от вирусов и угроз.|
|дефендерсекуритицентердисаблеаккаунтуи|Логический|Используется для отключения отображения области защиты учетных записей.|
|дефендерсекуритицентердисаблеклеартпмуи|Логический|Используется для отключения отображения кнопки Очистить доверенный платформенный модуль.|
|дефендерсекуритицентердисаблехардвареуи|Логический|Используется для отключения отображения области аппаратной защиты.|
|дефендерсекуритицентердисабленотификатионареауи|Логический|Используется для отключения отображения элемента управления "область уведомлений". Для вступления этого параметра в силу пользователю необходимо выйти из системы и войти в нее, а затем перезагрузить компьютер.|
|дефендерсекуритицентердисаблерансомвареуи|Логический|Используется для отключения отображения области защиты от пошантажистом. |
|дефендерсекуритицентердисаблесекуребутуи|Логический|Используется для отключения отображения области безопасной загрузки в разделе Безопасность устройства.|
|дефендерсекуритицентердисаблетраублешутингуи|Логический|Используется для отключения отображения устранения неполадок процесса безопасности в разделе Безопасность устройства.|
|дефендерсекуритицентердисаблевулнераблетпмфирмвареупдатеуи|Логический|Используется для отключения отображения обновления микропрограммы доверенного платформенного модуля при обнаружении уязвимого программного обеспечения.|
|дефендерсекуритицентерорганизатиондисплайнаме|String|Имя компании, которое отображается для пользователей.|
|дефендерсекуритицентерхелпемаил|String|Адрес электронной почты, который отображается для пользователей.|
|дефендерсекуритицентерхелпфоне|String|Номер телефона или идентификатор Skype, который отображается для пользователей.|
|дефендерсекуритицентерхелпурл|String|URL-адрес портала справки это отображается для пользователей.|
|дефендерсекуритицентернотификатионсфромапп|[дефендерсекуритицентернотификатионсфромапптипе](../resources/intune-deviceconfig-defendersecuritycenternotificationsfromapptype.md)|Уведомления, отображаемые в отображаемых областях приложения. Возможные значения: `notConfigured`, `blockNoncriticalNotifications`, `blockAllNotifications`.|
|дефендерсекуритицентеритконтактдисплай|[дефендерсекуритицентеритконтактдисплайтипе](../resources/intune-deviceconfig-defendersecuritycenteritcontactdisplaytype.md)|Настройка места отображения контактной информации для конечных пользователей. Возможные значения: `notConfigured`, `displayInAppAndInNotifications`, `displayOnlyInApp`, `displayOnlyInNotifications`.|
|виндовсдефендертамперпротектион|[windowsDefenderTamperProtectionOptions](../resources/intune-deviceconfig-windowsdefendertamperprotectionoptions.md)|Настройка параметров Тамперпротектион для защитника Windows. Возможные значения: `notConfigured`, `enable`, `disable`.|
|firewallBlockStatefulFTP|Логический|Блокирует FTP-подключения к устройству с отслеживанием состояния.|
|firewallIdleTimeoutForSecurityAssociationInSeconds|Int32|Настраивает время ожидания для сопоставлений безопасности в секундах от 300 до 3600 включительно. По истечении этого срока сопоставления безопасности перестают действовать и удаляются. Допустимые значения: от 300 до 3600|
|firewallPreSharedKeyEncodingMethod|[фиреваллпрешаредкэйенкодингмесодтипе](../resources/intune-deviceconfig-firewallpresharedkeyencodingmethodtype.md)|Выберите используемую кодировку с общим ключом. Возможные значения: `deviceDefault`, `none`, `utF8`.|
|firewallIPSecExemptionsAllowNeighborDiscovery|Логический|Настраивает исключения IPSec для разрешения обнаружения соседей. Коды типов ICMP IPv6.|
|firewallIPSecExemptionsAllowICMP|Логический|Настраивает исключения IPSec для разрешения ICMP|
|firewallIPSecExemptionsAllowRouterDiscovery|Логический|Настраивает исключения IPSec для разрешения обнаружения маршрутизаторов. Коды типов ICMP IPv6.|
|firewallIPSecExemptionsAllowDHCP|Логический|Настраивает исключения IPSec для разрешения DHCP-трафика IPv4 и IPv6|
|firewallCertificateRevocationListCheckMethod|[фиреваллцертификатеревокатионлистчеккмесодтипе](../resources/intune-deviceconfig-firewallcertificaterevocationlistcheckmethodtype.md)|Укажите способ применения списка отзыва сертификатов. Возможные значения: `deviceDefault`, `none`, `attempt`, `require`.|
|firewallMergeKeyingModuleSettings|Boolean|Если модуль ключей поддерживает не весь набор проверки подлинности, дайте ему указание игнорировать только неподдерживаемые пакеты, а не весь набор|
|firewallPacketQueueingMethod|[фиреваллпаккеткуеуеингмесодтипе](../resources/intune-deviceconfig-firewallpacketqueueingmethodtype.md)|Настраивает способ применения очередей пакетов в сценарии туннельного шлюза. Возможные значения: `deviceDefault`, `disabled`, `queueInbound`, `queueOutbound`, `queueBoth`.|
|firewallProfileDomain|[windowsFirewallNetworkProfile](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|Настраивает параметры профиля брандмауэра для доменных сетей|
|firewallProfilePublic|[windowsFirewallNetworkProfile](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|Настраивает параметры профиля брандмауэра для общедоступных сетей|
|firewallProfilePrivate|[windowsFirewallNetworkProfile](../resources/intune-deviceconfig-windowsfirewallnetworkprofile.md)|Настраивает параметры профиля брандмауэра для частных сетей|
|дефендерадобереадерлаунччилдпроцесс|[дефендерпротектионтипе](../resources/intune-deviceconfig-defenderprotectiontype.md)|Значение, указывающее поведение Adobe Reader при создании дочерних процессов. Возможные значения: `userDefined`, `enable`, `auditMode`.|
|defenderAttackSurfaceReductionExcludedPaths|Коллекция String|Список файлов EXE и папок, которые следует исключить из правил сокращения направлений атак|
|дефендероффицеаппсосерпроцессинжектионтипе|[дефендераттакксурфацетипе](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|Значение, указывающее поведение приложений Office, добавляемых в другие процессы. Возможные значения: `userDefined`, `block`, `auditMode`.|
|дефендероффицеаппсосерпроцессинжектион|[дефендерпротектионтипе](../resources/intune-deviceconfig-defenderprotectiontype.md)|Значение, указывающее поведение приложений Office, добавляемых в другие процессы. Возможные значения: `userDefined`, `enable`, `auditMode`.|
|дефендероффицекоммуникатионаппслаунччилдпроцесс|[дефендерпротектионтипе](../resources/intune-deviceconfig-defenderprotectiontype.md)|Значение, определяющее поведение приложений для связи с Office, включая Microsoft Outlook, от создания дочерних процессов. Возможные значения: `userDefined`, `enable`, `auditMode`.|
|дефендероффицеаппсексекутаблеконтенткреатионорлаунчтипе|[дефендераттакксурфацетипе](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|Значение, указывающее поведение приложений и макросов Office при создании или запуске исполняемого контента. Возможные значения: `userDefined`, `block`, `auditMode`.|
|дефендероффицеаппсексекутаблеконтенткреатионорлаунч|[дефендерпротектионтипе](../resources/intune-deviceconfig-defenderprotectiontype.md)|Значение, указывающее поведение приложений и макросов Office при создании или запуске исполняемого контента. Возможные значения: `userDefined`, `enable`, `auditMode`.|
|дефендероффицеаппслаунччилдпроцесстипе|[дефендераттакксурфацетипе](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|Значение, указывающее поведение запуска приложения Office для дочерних процессов. Возможные значения: `userDefined`, `block`, `auditMode`.|
|дефендероффицеаппслаунччилдпроцесс|[дефендерпротектионтипе](../resources/intune-deviceconfig-defenderprotectiontype.md)|Значение, указывающее поведение запуска приложения Office для дочерних процессов. Возможные значения: `userDefined`, `enable`, `auditMode`.|
|defenderOfficeMacroCodeAllowWin32ImportsType|[дефендераттакксурфацетипе](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|Значение, указывающее поведение импорта Win32 из кода макросов в Office. Возможные значения: `userDefined`, `block`, `auditMode`.|
|defenderOfficeMacroCodeAllowWin32Imports|[дефендерпротектионтипе](../resources/intune-deviceconfig-defenderprotectiontype.md)|Значение, указывающее поведение импорта Win32 из кода макросов в Office. Возможные значения: `userDefined`, `enable`, `auditMode`.|
|дефендерскриптобфускатедмакрокодетипе|[дефендераттакксурфацетипе](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|Значение, определяющее поведение кода "замаскированный JS/VBS/PS/макрос". Возможные значения: `userDefined`, `block`, `auditMode`.|
|дефендерскриптобфускатедмакрокоде|[дефендерпротектионтипе](../resources/intune-deviceconfig-defenderprotectiontype.md)|Значение, определяющее поведение кода "замаскированный JS/VBS/PS/макрос". Возможные значения: `userDefined`, `enable`, `auditMode`.|
|дефендерскриптдовнлоадедпайлоадексекутионтипе|[дефендераттакксурфацетипе](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|Значение, определяющее поведение JS-и VBS-данных, загруженных из Интернета. Возможные значения: `userDefined`, `block`, `auditMode`.|
|дефендерскриптдовнлоадедпайлоадексекутион|[дефендерпротектионтипе](../resources/intune-deviceconfig-defenderprotectiontype.md)|Значение, определяющее поведение JS-и VBS-данных, загруженных из Интернета. Возможные значения: `userDefined`, `enable`, `auditMode`.|
|дефендерпревенткредентиалстеалингтипе|[дефендерпротектионтипе](../resources/intune-deviceconfig-defenderprotectiontype.md)|Значение, указывающее, разрешено ли перенос учетных данных из подсистемы локального центра безопасности Windows. Возможные значения: `userDefined`, `enable`, `auditMode`.|
|дефендерпроцесскреатионтипе|[дефендераттакксурфацетипе](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|Значение, указывающее ответ на создание процессов, исходящих от команд PSExec и WMI. Возможные значения: `userDefined`, `block`, `auditMode`.|
|дефендерпроцесскреатион|[дефендерпротектионтипе](../resources/intune-deviceconfig-defenderprotectiontype.md)|Значение, указывающее ответ на создание процессов, исходящих от команд PSExec и WMI. Возможные значения: `userDefined`, `enable`, `auditMode`.|
|дефендерунтрустедусбпроцесстипе|[дефендераттакксурфацетипе](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|Значение, указывающее ответ на недоверенные и неподписанные процессы, которые запускаются с USB. Возможные значения: `userDefined`, `block`, `auditMode`.|
|дефендерунтрустедусбпроцесс|[дефендерпротектионтипе](../resources/intune-deviceconfig-defenderprotectiontype.md)|Значение, указывающее ответ на недоверенные и неподписанные процессы, которые запускаются с USB. Возможные значения: `userDefined`, `enable`, `auditMode`.|
|дефендерунтрустедексекутаблетипе|[дефендераттакксурфацетипе](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|Значение, указывающее ответ на исполняемые файлы, которые не отвечают условиям преобладание, возраст или доверенного списка. Возможные значения: `userDefined`, `block`, `auditMode`.|
|дефендерунтрустедексекутабле|[дефендерпротектионтипе](../resources/intune-deviceconfig-defenderprotectiontype.md)|Значение, указывающее ответ на исполняемые файлы, которые не отвечают условиям преобладание, возраст или доверенного списка. Возможные значения: `userDefined`, `enable`, `auditMode`.|
|дефендеремаилконтентексекутионтипе|[дефендераттакксурфацетипе](../resources/intune-deviceconfig-defenderattacksurfacetype.md)|Значение, указывающее, следует ли удалять исполняемые файлы (exe, DLL, PS, JS, VBS и т. д.) из электронной почты (почтовая или почтовая программа). Возможные значения: `userDefined`, `block`, `auditMode`.|
|дефендеремаилконтентексекутион|[дефендерпротектионтипе](../resources/intune-deviceconfig-defenderprotectiontype.md)|Значение, указывающее, следует ли удалять исполняемые файлы (exe, DLL, PS, JS, VBS и т. д.) из электронной почты (почтовая или почтовая программа). Возможные значения: `userDefined`, `enable`, `auditMode`.|
|дефендерадванцедрансомеварепротектионтипе|[дефендерпротектионтипе](../resources/intune-deviceconfig-defenderprotectiontype.md)|Значение, указывающее на использование расширенной защиты в рансомеваре. Возможные значения: `userDefined`, `enable`, `auditMode`.|
|дефендергуардмифолдерстипе|[фолдерпротектионтипе](../resources/intune-deviceconfig-folderprotectiontype.md)|Значение, указывающее поведение защищенных папок. Возможные значения: `userDefined`, `enable`, `auditMode`, `blockDiskModification`, `auditDiskModification`.|
|defenderGuardedFoldersAllowedAppPaths|Коллекция String|Список путей к файлам EXE, которым разрешен доступ к защищенным папкам|
|defenderAdditionalGuardedFolders|Коллекция String|Список путей к папкам, которые следует добавить в список защищенных папок|
|дефендернетворкпротектионтипе|[дефендерпротектионтипе](../resources/intune-deviceconfig-defenderprotectiontype.md)|Значение, указывающее поведение Нетворкпротектион. Возможные значения: `userDefined`, `enable`, `auditMode`.|
|defenderExploitProtectionXml|Binary|XML-файл с информацией о защите от эксплойтов.|
|defenderExploitProtectionXmlFileName|String|Имя файла, из которого получено свойство DefenderExploitProtectionXml.|
|defenderSecurityCenterBlockExploitProtectionOverride|Логический|Указывает, следует ли запретить пользователю переопределять настройки защиты от эксплойтов.|
|appLockerApplicationControl|[апплоккераппликатионконтролтипе](../resources/intune-deviceconfig-applockerapplicationcontroltype.md)|Позволяет администратору выбирать разрешенные типы приложений для устройств. Возможные значения: `notConfigured`, `enforceComponentsAndStoreApps`, `auditComponentsAndStoreApps`, `enforceComponentsStoreAppsAndSmartlocker`, `auditComponentsStoreAppsAndSmartlocker`.|
|девицегуардлокалсистемаусоритикредентиалгуардсеттингс|[девицегуардлокалсистемаусоритикредентиалгуардтипе](../resources/intune-deviceconfig-deviceguardlocalsystemauthoritycredentialguardtype.md)|Включите Guard в учетных данных, когда включен уровень безопасности платформы с безопасной загрузкой и безопасностью на основе виртуализации. Возможные значения: `notConfigured`, `enableWithUEFILock`, `enableWithoutUEFILock`.|
|девицегуарденаблевиртуализатионбаседсекурити|Логический|Включает безопасность на основе виртуализации (VBS).|
|девицегуарденаблесекуребутвисдма|Логический|Это свойство будет устаревшим в 2019 мая и будет заменено свойством Девицегуардсекуребутвисдма. Указывает, включен ли уровень безопасности платформы при следующей перезагрузке.|
|девицегуардсекуребутвисдма|[secureBootWithDMAType](../resources/intune-deviceconfig-securebootwithdmatype.md)|Указывает, включен ли уровень безопасности платформы при следующей перезагрузке. Возможные значения: `notConfigured`, `withoutDMA`, `withDMA`.|
|девицегуардлаунчсистемгуард|[Включение](../resources/intune-shared-enablement.md)|Позволяет ИТ – администратору настраивать запуск системы защиты системы. Возможные значения: `notConfigured`, `enabled`, `disabled`.|
|smartScreenEnableInShell|Логический|Позволяет ИТ-администраторам настраивать SmartScreen для Windows.|
|smartScreenBlockOverrideForFiles|Логический|Позволяет ИТ-администраторам указывать, могут ли пользователи игнорировать предупреждения SmartScreen и запускать вредоносные файлы.|
|applicationGuardEnabled|Логический|Включение Application Guard в Защитнике Windows|
|applicationGuardEnabledOptions|[applicationGuardEnabledOptions](../resources/intune-deviceconfig-applicationguardenabledoptions.md)|Включение Application Guard в Защитнике Windows для более новых сборок Windows. Возможные значения: `notConfigured`, `enabledForEdge`, `enabledForOffice`, `enabledForEdgeAndOffice`.|
|applicationGuardBlockFileTransfer|[аппликатионгуардблоккфилетрансфертипе](../resources/intune-deviceconfig-applicationguardblockfiletransfertype.md)|Блокировать буфер обмена для передачи файла изображения, текстового файла или ни одного из них. Возможные значения: `notConfigured`, `blockImageAndTextFile`, `blockImageFile`, `blockNone`, `blockTextFile`.|
|applicationGuardBlockNonEnterpriseContent|Логический|Позволяет заблокировать загрузку некорпоративного контента, например сторонних подключаемых модулей, на корпоративных сайтах.|
|applicationGuardAllowPersistence|Логический|Позволяет разрешить сохранение пользовательских данных в контейнере App Guard (избранное, файлы cookie, веб-пароли и т. д.).|
|applicationGuardForceAuditing|Логический|Эта политика позволяет сохранять журналы и события Windows (попытки входа и выхода, использование привилегий, установка программного обеспечения, системные изменения и т. д.) для обеспечения безопасности и соответствия требованиям.|
|applicationGuardBlockClipboardSharing|[аппликатионгуардблоккклипбоардшарингтипе](../resources/intune-deviceconfig-applicationguardblockclipboardsharingtype.md)|Позволяет заблокировать передачу данных с узла в контейнер или с контейнера в узел через буфер обмена. Возможные значения: `notConfigured`, `blockBoth`, `blockHostToContainer`, `blockContainerToHost`, `blockNone`.|
|applicationGuardAllowPrintToPDF|Логический|Позволяет разрешить печать в PDF из контейнера.|
|applicationGuardAllowPrintToXPS|Логический|Позволяет разрешить печать в XPS из контейнера.|
|applicationGuardAllowPrintToLocalPrinters|Логический|Позволяет разрешить печать на локальных принтерах из контейнера.|
|applicationGuardAllowPrintToNetworkPrinters|Логический|Позволяет разрешить печать на сетевых принтерах из контейнера.|
|аппликатионгуардалловвиртуалгпу|Логический|Разрешить приложению Application Guard использовать виртуальный GPU|
|аппликатионгуардалловфилесавеонхост|Логический|Разрешить пользователям скачивать файлы из EDGE в контейнере Application Guard и сохранять их в файловой системе узла|
|битлоккералловстандардусеренкриптион|Логический|Позволяет администратору разрешить обычным пользователям включать енкрпитион во время присоединения к Azure AD.|
|bitLockerDisableWarningForOtherDiskEncryption|Логический|Позволяет администратору отключить предупреждение о другом методе шифрования диска на компьютерах пользователей.|
|bitLockerEnableStorageCardEncryptionOnMobile|Boolean|Позволяет администратору требовать включения шифрования с помощью BitLocker. Эта политика действительна только для мобильных устройств.|
|bitLockerEncryptDevice|Boolean|Позволяет администратору требовать включения шифрования с помощью BitLocker.|
|bitLockerSystemDrivePolicy|[bitLockerSystemDrivePolicy](../resources/intune-deviceconfig-bitlockersystemdrivepolicy.md)|Политика системного диска BitLocker.|
|bitLockerFixedDrivePolicy|[bitLockerFixedDrivePolicy](../resources/intune-deviceconfig-bitlockerfixeddrivepolicy.md);|Политика фиксированного диска BitLocker.|
|bitLockerRemovableDrivePolicy|[bitLockerRemovableDrivePolicy](../resources/intune-deviceconfig-bitlockerremovabledrivepolicy.md)|Политика BitLocker в отношении съемных дисков.|
|битлоккеррековерипассвордротатион|[bitLockerRecoveryPasswordRotationType](../resources/intune-deviceconfig-bitlockerrecoverypasswordrotationtype.md)|Этот параметр инициирует поворот пароля восстановления на основе клиента после восстановления диска ОС (с помощью BOOTMGR или WinRE). Возможные значения: `notConfigured`, `disabled`, `enabledForAzureAd`, `enabledForAzureAdAndHybrid`.|
|дефендердисаблесканарчивефилес|Логический|Разрешает или запрещает сканирование архивов.|
|дефендералловсканарчивефилес|Логический|Разрешает или запрещает сканирование архивов.|
|дефендердисаблебехавиормониторинг|Логический|Разрешает или запрещает функции мониторинга режима защитника Windows.|
|дефендералловбехавиормониторинг|Логический|Разрешает или запрещает функции мониторинга режима защитника Windows.|
|дефендердисаблеклаудпротектион|Логический|Чтобы лучше защитить компьютер, защитник Windows будет отправлять в корпорацию Майкрософт сведения обо всех обнаруженных неполадках. Корпорация Майкрософт проанализирует эти сведения, Узнайте больше об ошибках, которые могут повлиять на ваших клиентов и других пользователей, и предложит улучшенные решения.|
|дефендералловклаудпротектион|Логический|Чтобы лучше защитить компьютер, защитник Windows будет отправлять в корпорацию Майкрософт сведения обо всех обнаруженных неполадках. Корпорация Майкрософт проанализирует эти сведения, Узнайте больше об ошибках, которые могут повлиять на ваших клиентов и других пользователей, и предложит улучшенные решения.|
|дефендеренаблесканинкомингмаил|Логический|Разрешает или запрещает сканирование электронной почты.|
|дефендеренаблесканмаппеднетворкдривесдурингфуллскан|Логический|Разрешает или запрещает полное сканирование подключенных сетевых дисков.|
|дефендердисаблесканремовабледривесдурингфуллскан|Логический|Разрешает или запрещает полное сканирование съемных дисков. Во время быстрого сканирования съемные диски все еще могут сканироваться.|
|дефендералловсканремовабледривесдурингфуллскан|Логический|Разрешает или запрещает полное сканирование съемных дисков. Во время быстрого сканирования съемные диски все еще могут сканироваться.|
|дефендердисаблескандовнлоадс|Логический|Разрешает или запрещает функции защиты ИОАВП защитника Windows.|
|дефендералловскандовнлоадс|Логический|Разрешает или запрещает функции защиты ИОАВП защитника Windows.|
|дефендердисаблеинтрусионпревентионсистем|Логический|Разрешает или запрещает функции предотвращения вторжения в Защитнике Windows.|
|дефендералловинтрусионпревентионсистем|Логический|Разрешает или запрещает функции предотвращения вторжения в Защитнике Windows.|
|дефендердисаблеонакцесспротектион|Логический|Разрешает или запрещает защитник Windows для функций защиты доступа.|
|дефендералловонакцесспротектион|Логический|Разрешает или запрещает защитник Windows для функций защиты доступа.|
|дефендердисаблереалтимемониторинг|Логический|Разрешает или запрещает функции мониторинга в режиме реального времени защитник Windows.|
|дефендералловреалтимемониторинг|Логический|Разрешает или запрещает функции мониторинга в режиме реального времени защитник Windows.|
|дефендердисаблесканнетворкфилес|Логический|Разрешает или запрещает сканирование сетевых файлов.|
|дефендералловсканнетворкфилес|Логический|Разрешает или запрещает сканирование сетевых файлов.|
|дефендердисаблесканскриптслоадедининтернетексплорер|Логический|Разрешает или запрещает функцию сканирования сценариев защитника Windows.|
|дефендералловсканскриптслоадедининтернетексплорер|Логический|Разрешает или запрещает функцию сканирования сценариев защитника Windows.|
|defenderBlockEndUserAccess|Boolean|Разрешает или запрещает пользователям доступ к пользовательскому интерфейсу защитника Windows. Если этот флажок не разрешен, все уведомления защитника Windows также будут подавляться.|
|дефендералловендусеракцесс|Логический|Разрешает или запрещает пользователям доступ к пользовательскому интерфейсу защитника Windows. Если этот флажок не разрешен, все уведомления защитника Windows также будут подавляться.|
|дефендерсканмакскпуперцентаже|Int32|Представляет средний коэффициент загрузки ЦП для сканирования защитником Windows (в процентах). Значение по умолчанию равно 50. Допустимые значения: от 0 до 100|
|дефендерчеккфорсигнатуресбефореруннингскан|Логический|Этот параметр политики позволяет управлять тем, будет ли выполняться проверка новых определений вирусов и программ-шпионов перед выполнением проверки.|
|defenderCloudBlockLevel|[дефендерклаудблокклевелтипе](../resources/intune-deviceconfig-defendercloudblockleveltype.md)|Добавлено в Windows 10 версии 1709. Этот параметр политики определяет, как активно антивирусная программа "Защитник Windows" будет блокировать и сканировать подозрительные файлы. Тип значения: целое число. Для работы этой функции необходимо включить параметр "присоединение к Microsoft MAPS". Возможные значения: `notConfigured`, `high`, `highPlus`, `zeroTolerance`.|
|дефендерклаудекстендедтимеаутинсекондс|Int32|Добавлено в Windows 10 версии 1709. Эта функция позволяет антивирусной программе "Защитник Windows" заблокировать подозрительный файл размером до 60 секунд и проверить его в облаке, чтобы убедиться, что он безопасен. Тип значения: целое число, Range — 0-50. Эта функция зависит от трех других параметров карт, которые должны быть включены — "Настройка блока при первом пошаговом отображении"; " Присоединяйтесь к Microsoft MAPS "; "Отправлять образцы файлов, когда необходим дальнейший анализ". Допустимые значения: от 0 до 50.|
|defenderDaysBeforeDeletingQuarantinedMalware|Int32|Период времени (в днях), в течение которого элементы, помещенные в карантин, будут храниться в системе. Допустимые значения: от 0 до 90.|
|дефендердисаблекатчупфуллскан|Логический|Этот параметр политики позволяет настроить поиск по расписанию для полного сканирования. Вторичное сканирование — это сканирование, которое инициируется из-за пропускной ошибки запланированной проверки. Обычно эти запланированные проверки пропущены, так как компьютер был отключен в запланированное время.|
|дефендердисаблекатчупкуиккскан|Логический|Этот параметр политики позволяет настроить дополнительные проверки для запланированных быстрых проверок. Вторичное сканирование — это сканирование, которое инициируется из-за пропускной ошибки запланированной проверки. Обычно эти запланированные проверки пропущены, так как компьютер был отключен в запланированное время.|
|дефендеренаблеловкпуприорити|Логический|Этот параметр политики позволяет включать или отключать минимальный приоритет ЦП для запланированных проверок.|
|defenderFileExtensionsToExclude|Коллекция String|Расширения файлов, которые необходимо исключить из проверки и защиты в режиме реального времени.|
|defenderFilesAndFoldersToExclude|Коллекция String|Файлы и папки, которые необходимо исключить из проверки и защиты в режиме реального времени.|
|defenderProcessesToExclude|Коллекция String|Процессы, которые необходимо исключить из проверки и защиты в режиме реального времени.|
|дефендерпотентиаллюнвантедаппактион|[дефендерпротектионтипе](../resources/intune-deviceconfig-defenderprotectiontype.md)|Добавлено в Windows 10 версии 1607. Задает уровень обнаружения для потенциально нежелательных приложений (Пуас). Защитник Windows предупреждает вас о том, что загружается потенциально нежелательное программное обеспечение, или пытается установить себя на компьютер. Возможные значения: `userDefined`, `enable`, `auditMode`.|
|дефендерскандиректион|[defenderRealtimeScanDirection](../resources/intune-deviceconfig-defenderrealtimescandirection.md)|Определяет, какие наборы файлов следует отслеживать. Возможные значения: `monitorAllFiles`, `monitorIncomingFilesOnly`, `monitorOutgoingFilesOnly`.|
|defenderScanType|[defenderScanType](../resources/intune-deviceconfig-defenderscantype.md)|Позволяет выбрать, следует ли выполнять быструю или полную проверку. Возможные значения: `userDefined`, `disabled`, `quick`, `full`.|
|defenderScheduledQuickScanTime|TimeOfDay|Выбирает время суток, которое должно выполняться при запуске быстрого сканирования защитника Windows. Например, значение 0 = 12:00AM, значение 60 = 1:00AM, значение 120 = 2:00 и т. д., вплоть до значения 1380 = 11:00PM. Значение по умолчанию — 120|
|дефендерсчедуледскандай|[виклисчедуле](../resources/intune-deviceconfig-weeklyschedule.md)|Выбирает день запуска проверки защитником Windows. Возможные значения: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`, `noScheduledScan`.|
|defenderScheduledScanTime|TimeOfDay|Выбирает время суток, в течение которого должно выполняться сканирование защитника Windows.|
|defenderSignatureUpdateIntervalInHours|Int32|Указывает интервал (в часах), который будет использоваться для проверки подписей, поэтому вместо использования Счедуледай и Счедулетиме проверка новых подписей будет установлена в соответствии с интервалом. Допустимые значения: от 0 до 24.|
|defenderSubmitSamplesConsentType|[defenderSubmitSamplesConsentType](../resources/intune-deviceconfig-defendersubmitsamplesconsenttype.md);|Проверка уровня согласия пользователя в Защитнике Windows для отправки данных. Возможные значения: `sendSafeSamplesAutomatically`, `alwaysPrompt`, `neverSend`, `sendAllSamplesAutomatically`.|
|defenderDetectedMalwareActions|[defenderDetectedMalwareActions](../resources/intune-deviceconfig-defenderdetectedmalwareactions.md)|Позволяет администратору указать допустимые уровни серьезности угроз и соответствующий идентификатор действия по умолчанию.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|groupAssignments|Коллекция [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)|Список назначений групп для профиля конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|assignments|Коллекция [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|Список назначений для профиля конфигурации устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceStatuses|Коллекция [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)|Состояние установки конфигурации для каждого устройства. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|userStatuses|Коллекция [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md)|Состояние установки конфигурации устройств пользователем. Наследуется от объекта [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|Обзор состояния конфигурации устройств. Наследуется от [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|Обзор состояния конфигурации устройств для пользователей. Наследуется от [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|
|deviceSettingStateSummaries|Коллекция [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)|Сводка данных о состоянии настройки конфигурации устройств. Наследуется от [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md).|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windows10EndpointProtectionConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows10EndpointProtectionConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "String"
    ],
    "name": "String",
    "ruleType": "String"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "String",
    "maxOSVersion": "String",
    "name": "String",
    "ruleType": "String"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "String",
    "name": "String",
    "ruleType": "String"
  },
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024,
  "dmaGuardDeviceEnumerationPolicy": "String",
  "firewallRules": [
    {
      "@odata.type": "microsoft.graph.windowsFirewallRule",
      "displayName": "String",
      "description": "String",
      "packageFamilyName": "String",
      "filePath": "String",
      "serviceName": "String",
      "protocol": 1024,
      "localPortRanges": [
        "String"
      ],
      "remotePortRanges": [
        "String"
      ],
      "localAddressRanges": [
        "String"
      ],
      "remoteAddressRanges": [
        "String"
      ],
      "profileTypes": "String",
      "action": "String",
      "trafficDirection": "String",
      "interfaceTypes": "String",
      "edgeTraversal": "String",
      "localUserAuthorizations": "String"
    }
  ],
  "userRightsAccessCredentialManagerAsTrustedCaller": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsAllowAccessFromNetwork": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsBlockAccessFromNetwork": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsActAsPartOfTheOperatingSystem": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsLocalLogOn": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsDenyLocalLogOn": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsBackupData": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsChangeSystemTime": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsCreateGlobalObjects": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsCreatePageFile": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsCreatePermanentSharedObjects": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsCreateSymbolicLinks": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsCreateToken": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsDebugPrograms": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsRemoteDesktopServicesLogOn": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsDelegation": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsGenerateSecurityAudits": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsImpersonateClient": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsIncreaseSchedulingPriority": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsLoadUnloadDrivers": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsLockMemory": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsManageAuditingAndSecurityLogs": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsManageVolumes": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsModifyFirmwareEnvironment": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsModifyObjectLabels": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsProfileSingleProcess": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsRemoteShutdown": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsRestoreData": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "userRightsTakeOwnership": {
    "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting",
    "state": "String",
    "localUsersOrGroups": [
      {
        "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
        "name": "String",
        "description": "String",
        "securityIdentifier": "String"
      }
    ]
  },
  "xboxServicesEnableXboxGameSaveTask": true,
  "xboxServicesAccessoryManagementServiceStartupMode": "String",
  "xboxServicesLiveAuthManagerServiceStartupMode": "String",
  "xboxServicesLiveGameSaveServiceStartupMode": "String",
  "xboxServicesLiveNetworkingServiceStartupMode": "String",
  "localSecurityOptionsBlockMicrosoftAccounts": true,
  "localSecurityOptionsBlockRemoteLogonWithBlankPassword": true,
  "localSecurityOptionsDisableAdministratorAccount": true,
  "localSecurityOptionsAdministratorAccountName": "String",
  "localSecurityOptionsDisableGuestAccount": true,
  "localSecurityOptionsGuestAccountName": "String",
  "localSecurityOptionsAllowUndockWithoutHavingToLogon": true,
  "localSecurityOptionsBlockUsersInstallingPrinterDrivers": true,
  "localSecurityOptionsBlockRemoteOpticalDriveAccess": true,
  "localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUser": "String",
  "localSecurityOptionsMachineInactivityLimit": 1024,
  "localSecurityOptionsMachineInactivityLimitInMinutes": 1024,
  "localSecurityOptionsDoNotRequireCtrlAltDel": true,
  "localSecurityOptionsHideLastSignedInUser": true,
  "localSecurityOptionsHideUsernameAtSignIn": true,
  "localSecurityOptionsLogOnMessageTitle": "String",
  "localSecurityOptionsLogOnMessageText": "String",
  "localSecurityOptionsAllowPKU2UAuthenticationRequests": true,
  "localSecurityOptionsAllowRemoteCallsToSecurityAccountsManagerHelperBool": true,
  "localSecurityOptionsAllowRemoteCallsToSecurityAccountsManager": "String",
  "localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedClients": "String",
  "localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedServers": "String",
  "lanManagerAuthenticationLevel": "String",
  "lanManagerWorkstationDisableInsecureGuestLogons": true,
  "localSecurityOptionsClearVirtualMemoryPageFile": true,
  "localSecurityOptionsAllowSystemToBeShutDownWithoutHavingToLogOn": true,
  "localSecurityOptionsAllowUIAccessApplicationElevation": true,
  "localSecurityOptionsVirtualizeFileAndRegistryWriteFailuresToPerUserLocations": true,
  "localSecurityOptionsOnlyElevateSignedExecutables": true,
  "localSecurityOptionsAdministratorElevationPromptBehavior": "String",
  "localSecurityOptionsStandardUserElevationPromptBehavior": "String",
  "localSecurityOptionsSwitchToSecureDesktopWhenPromptingForElevation": true,
  "localSecurityOptionsDetectApplicationInstallationsAndPromptForElevation": true,
  "localSecurityOptionsAllowUIAccessApplicationsForSecureLocations": true,
  "localSecurityOptionsUseAdminApprovalMode": true,
  "localSecurityOptionsUseAdminApprovalModeForAdministrators": true,
  "localSecurityOptionsInformationShownOnLockScreen": "String",
  "localSecurityOptionsInformationDisplayedOnLockScreen": "String",
  "localSecurityOptionsDisableClientDigitallySignCommunicationsIfServerAgrees": true,
  "localSecurityOptionsClientDigitallySignCommunicationsAlways": true,
  "localSecurityOptionsClientSendUnencryptedPasswordToThirdPartySMBServers": true,
  "localSecurityOptionsDisableServerDigitallySignCommunicationsAlways": true,
  "localSecurityOptionsDisableServerDigitallySignCommunicationsIfClientAgrees": true,
  "localSecurityOptionsRestrictAnonymousAccessToNamedPipesAndShares": true,
  "localSecurityOptionsDoNotAllowAnonymousEnumerationOfSAMAccounts": true,
  "localSecurityOptionsAllowAnonymousEnumerationOfSAMAccountsAndShares": true,
  "localSecurityOptionsDoNotStoreLANManagerHashValueOnNextPasswordChange": true,
  "localSecurityOptionsSmartCardRemovalBehavior": "String",
  "defenderSecurityCenterDisableAppBrowserUI": true,
  "defenderSecurityCenterDisableFamilyUI": true,
  "defenderSecurityCenterDisableHealthUI": true,
  "defenderSecurityCenterDisableNetworkUI": true,
  "defenderSecurityCenterDisableVirusUI": true,
  "defenderSecurityCenterDisableAccountUI": true,
  "defenderSecurityCenterDisableClearTpmUI": true,
  "defenderSecurityCenterDisableHardwareUI": true,
  "defenderSecurityCenterDisableNotificationAreaUI": true,
  "defenderSecurityCenterDisableRansomwareUI": true,
  "defenderSecurityCenterDisableSecureBootUI": true,
  "defenderSecurityCenterDisableTroubleshootingUI": true,
  "defenderSecurityCenterDisableVulnerableTpmFirmwareUpdateUI": true,
  "defenderSecurityCenterOrganizationDisplayName": "String",
  "defenderSecurityCenterHelpEmail": "String",
  "defenderSecurityCenterHelpPhone": "String",
  "defenderSecurityCenterHelpURL": "String",
  "defenderSecurityCenterNotificationsFromApp": "String",
  "defenderSecurityCenterITContactDisplay": "String",
  "windowsDefenderTamperProtection": "String",
  "firewallBlockStatefulFTP": true,
  "firewallIdleTimeoutForSecurityAssociationInSeconds": 1024,
  "firewallPreSharedKeyEncodingMethod": "String",
  "firewallIPSecExemptionsAllowNeighborDiscovery": true,
  "firewallIPSecExemptionsAllowICMP": true,
  "firewallIPSecExemptionsAllowRouterDiscovery": true,
  "firewallIPSecExemptionsAllowDHCP": true,
  "firewallCertificateRevocationListCheckMethod": "String",
  "firewallMergeKeyingModuleSettings": true,
  "firewallPacketQueueingMethod": "String",
  "firewallProfileDomain": {
    "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile",
    "firewallEnabled": "String",
    "stealthModeRequired": true,
    "stealthModeBlocked": true,
    "incomingTrafficRequired": true,
    "incomingTrafficBlocked": true,
    "unicastResponsesToMulticastBroadcastsRequired": true,
    "unicastResponsesToMulticastBroadcastsBlocked": true,
    "inboundNotificationsRequired": true,
    "inboundNotificationsBlocked": true,
    "authorizedApplicationRulesFromGroupPolicyMerged": true,
    "authorizedApplicationRulesFromGroupPolicyNotMerged": true,
    "globalPortRulesFromGroupPolicyMerged": true,
    "globalPortRulesFromGroupPolicyNotMerged": true,
    "connectionSecurityRulesFromGroupPolicyMerged": true,
    "connectionSecurityRulesFromGroupPolicyNotMerged": true,
    "outboundConnectionsRequired": true,
    "outboundConnectionsBlocked": true,
    "inboundConnectionsRequired": true,
    "inboundConnectionsBlocked": true,
    "securedPacketExemptionAllowed": true,
    "securedPacketExemptionBlocked": true,
    "policyRulesFromGroupPolicyMerged": true,
    "policyRulesFromGroupPolicyNotMerged": true
  },
  "firewallProfilePublic": {
    "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile",
    "firewallEnabled": "String",
    "stealthModeRequired": true,
    "stealthModeBlocked": true,
    "incomingTrafficRequired": true,
    "incomingTrafficBlocked": true,
    "unicastResponsesToMulticastBroadcastsRequired": true,
    "unicastResponsesToMulticastBroadcastsBlocked": true,
    "inboundNotificationsRequired": true,
    "inboundNotificationsBlocked": true,
    "authorizedApplicationRulesFromGroupPolicyMerged": true,
    "authorizedApplicationRulesFromGroupPolicyNotMerged": true,
    "globalPortRulesFromGroupPolicyMerged": true,
    "globalPortRulesFromGroupPolicyNotMerged": true,
    "connectionSecurityRulesFromGroupPolicyMerged": true,
    "connectionSecurityRulesFromGroupPolicyNotMerged": true,
    "outboundConnectionsRequired": true,
    "outboundConnectionsBlocked": true,
    "inboundConnectionsRequired": true,
    "inboundConnectionsBlocked": true,
    "securedPacketExemptionAllowed": true,
    "securedPacketExemptionBlocked": true,
    "policyRulesFromGroupPolicyMerged": true,
    "policyRulesFromGroupPolicyNotMerged": true
  },
  "firewallProfilePrivate": {
    "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile",
    "firewallEnabled": "String",
    "stealthModeRequired": true,
    "stealthModeBlocked": true,
    "incomingTrafficRequired": true,
    "incomingTrafficBlocked": true,
    "unicastResponsesToMulticastBroadcastsRequired": true,
    "unicastResponsesToMulticastBroadcastsBlocked": true,
    "inboundNotificationsRequired": true,
    "inboundNotificationsBlocked": true,
    "authorizedApplicationRulesFromGroupPolicyMerged": true,
    "authorizedApplicationRulesFromGroupPolicyNotMerged": true,
    "globalPortRulesFromGroupPolicyMerged": true,
    "globalPortRulesFromGroupPolicyNotMerged": true,
    "connectionSecurityRulesFromGroupPolicyMerged": true,
    "connectionSecurityRulesFromGroupPolicyNotMerged": true,
    "outboundConnectionsRequired": true,
    "outboundConnectionsBlocked": true,
    "inboundConnectionsRequired": true,
    "inboundConnectionsBlocked": true,
    "securedPacketExemptionAllowed": true,
    "securedPacketExemptionBlocked": true,
    "policyRulesFromGroupPolicyMerged": true,
    "policyRulesFromGroupPolicyNotMerged": true
  },
  "defenderAdobeReaderLaunchChildProcess": "String",
  "defenderAttackSurfaceReductionExcludedPaths": [
    "String"
  ],
  "defenderOfficeAppsOtherProcessInjectionType": "String",
  "defenderOfficeAppsOtherProcessInjection": "String",
  "defenderOfficeCommunicationAppsLaunchChildProcess": "String",
  "defenderOfficeAppsExecutableContentCreationOrLaunchType": "String",
  "defenderOfficeAppsExecutableContentCreationOrLaunch": "String",
  "defenderOfficeAppsLaunchChildProcessType": "String",
  "defenderOfficeAppsLaunchChildProcess": "String",
  "defenderOfficeMacroCodeAllowWin32ImportsType": "String",
  "defenderOfficeMacroCodeAllowWin32Imports": "String",
  "defenderScriptObfuscatedMacroCodeType": "String",
  "defenderScriptObfuscatedMacroCode": "String",
  "defenderScriptDownloadedPayloadExecutionType": "String",
  "defenderScriptDownloadedPayloadExecution": "String",
  "defenderPreventCredentialStealingType": "String",
  "defenderProcessCreationType": "String",
  "defenderProcessCreation": "String",
  "defenderUntrustedUSBProcessType": "String",
  "defenderUntrustedUSBProcess": "String",
  "defenderUntrustedExecutableType": "String",
  "defenderUntrustedExecutable": "String",
  "defenderEmailContentExecutionType": "String",
  "defenderEmailContentExecution": "String",
  "defenderAdvancedRansomewareProtectionType": "String",
  "defenderGuardMyFoldersType": "String",
  "defenderGuardedFoldersAllowedAppPaths": [
    "String"
  ],
  "defenderAdditionalGuardedFolders": [
    "String"
  ],
  "defenderNetworkProtectionType": "String",
  "defenderExploitProtectionXml": "binary",
  "defenderExploitProtectionXmlFileName": "String",
  "defenderSecurityCenterBlockExploitProtectionOverride": true,
  "appLockerApplicationControl": "String",
  "deviceGuardLocalSystemAuthorityCredentialGuardSettings": "String",
  "deviceGuardEnableVirtualizationBasedSecurity": true,
  "deviceGuardEnableSecureBootWithDMA": true,
  "deviceGuardSecureBootWithDMA": "String",
  "deviceGuardLaunchSystemGuard": "String",
  "smartScreenEnableInShell": true,
  "smartScreenBlockOverrideForFiles": true,
  "applicationGuardEnabled": true,
  "applicationGuardEnabledOptions": "String",
  "applicationGuardBlockFileTransfer": "String",
  "applicationGuardBlockNonEnterpriseContent": true,
  "applicationGuardAllowPersistence": true,
  "applicationGuardForceAuditing": true,
  "applicationGuardBlockClipboardSharing": "String",
  "applicationGuardAllowPrintToPDF": true,
  "applicationGuardAllowPrintToXPS": true,
  "applicationGuardAllowPrintToLocalPrinters": true,
  "applicationGuardAllowPrintToNetworkPrinters": true,
  "applicationGuardAllowVirtualGPU": true,
  "applicationGuardAllowFileSaveOnHost": true,
  "bitLockerAllowStandardUserEncryption": true,
  "bitLockerDisableWarningForOtherDiskEncryption": true,
  "bitLockerEnableStorageCardEncryptionOnMobile": true,
  "bitLockerEncryptDevice": true,
  "bitLockerSystemDrivePolicy": {
    "@odata.type": "microsoft.graph.bitLockerSystemDrivePolicy",
    "encryptionMethod": "String",
    "startupAuthenticationRequired": true,
    "startupAuthenticationBlockWithoutTpmChip": true,
    "startupAuthenticationTpmUsage": "String",
    "startupAuthenticationTpmPinUsage": "String",
    "startupAuthenticationTpmKeyUsage": "String",
    "startupAuthenticationTpmPinAndKeyUsage": "String",
    "minimumPinLength": 1024,
    "recoveryOptions": {
      "@odata.type": "microsoft.graph.bitLockerRecoveryOptions",
      "blockDataRecoveryAgent": true,
      "recoveryPasswordUsage": "String",
      "recoveryKeyUsage": "String",
      "hideRecoveryOptions": true,
      "enableRecoveryInformationSaveToStore": true,
      "recoveryInformationToStore": "String",
      "enableBitLockerAfterRecoveryInformationToStore": true
    },
    "prebootRecoveryEnableMessageAndUrl": true,
    "prebootRecoveryMessage": "String",
    "prebootRecoveryUrl": "String"
  },
  "bitLockerFixedDrivePolicy": {
    "@odata.type": "microsoft.graph.bitLockerFixedDrivePolicy",
    "encryptionMethod": "String",
    "requireEncryptionForWriteAccess": true,
    "recoveryOptions": {
      "@odata.type": "microsoft.graph.bitLockerRecoveryOptions",
      "blockDataRecoveryAgent": true,
      "recoveryPasswordUsage": "String",
      "recoveryKeyUsage": "String",
      "hideRecoveryOptions": true,
      "enableRecoveryInformationSaveToStore": true,
      "recoveryInformationToStore": "String",
      "enableBitLockerAfterRecoveryInformationToStore": true
    }
  },
  "bitLockerRemovableDrivePolicy": {
    "@odata.type": "microsoft.graph.bitLockerRemovableDrivePolicy",
    "encryptionMethod": "String",
    "requireEncryptionForWriteAccess": true,
    "blockCrossOrganizationWriteAccess": true
  },
  "bitLockerRecoveryPasswordRotation": "String",
  "defenderDisableScanArchiveFiles": true,
  "defenderAllowScanArchiveFiles": true,
  "defenderDisableBehaviorMonitoring": true,
  "defenderAllowBehaviorMonitoring": true,
  "defenderDisableCloudProtection": true,
  "defenderAllowCloudProtection": true,
  "defenderEnableScanIncomingMail": true,
  "defenderEnableScanMappedNetworkDrivesDuringFullScan": true,
  "defenderDisableScanRemovableDrivesDuringFullScan": true,
  "defenderAllowScanRemovableDrivesDuringFullScan": true,
  "defenderDisableScanDownloads": true,
  "defenderAllowScanDownloads": true,
  "defenderDisableIntrusionPreventionSystem": true,
  "defenderAllowIntrusionPreventionSystem": true,
  "defenderDisableOnAccessProtection": true,
  "defenderAllowOnAccessProtection": true,
  "defenderDisableRealTimeMonitoring": true,
  "defenderAllowRealTimeMonitoring": true,
  "defenderDisableScanNetworkFiles": true,
  "defenderAllowScanNetworkFiles": true,
  "defenderDisableScanScriptsLoadedInInternetExplorer": true,
  "defenderAllowScanScriptsLoadedInInternetExplorer": true,
  "defenderBlockEndUserAccess": true,
  "defenderAllowEndUserAccess": true,
  "defenderScanMaxCpuPercentage": 1024,
  "defenderCheckForSignaturesBeforeRunningScan": true,
  "defenderCloudBlockLevel": "String",
  "defenderCloudExtendedTimeoutInSeconds": 1024,
  "defenderDaysBeforeDeletingQuarantinedMalware": 1024,
  "defenderDisableCatchupFullScan": true,
  "defenderDisableCatchupQuickScan": true,
  "defenderEnableLowCpuPriority": true,
  "defenderFileExtensionsToExclude": [
    "String"
  ],
  "defenderFilesAndFoldersToExclude": [
    "String"
  ],
  "defenderProcessesToExclude": [
    "String"
  ],
  "defenderPotentiallyUnwantedAppAction": "String",
  "defenderScanDirection": "String",
  "defenderScanType": "String",
  "defenderScheduledQuickScanTime": "String (time of day)",
  "defenderScheduledScanDay": "String",
  "defenderScheduledScanTime": "String (time of day)",
  "defenderSignatureUpdateIntervalInHours": 1024,
  "defenderSubmitSamplesConsentType": "String",
  "defenderDetectedMalwareActions": {
    "@odata.type": "microsoft.graph.defenderDetectedMalwareActions",
    "lowSeverity": "String",
    "moderateSeverity": "String",
    "highSeverity": "String",
    "severeSeverity": "String"
  }
}
```



