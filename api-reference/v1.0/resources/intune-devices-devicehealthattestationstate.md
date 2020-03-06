---
title: Тип ресурса deviceHealthAttestationState
description: Пока не задокументировано.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d56cc2689a9987f99ac7abd7a132ff1526bf88c0
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42532220"
---
# <a name="devicehealthattestationstate-resource-type"></a>Тип ресурса deviceHealthAttestationState

Пространство имен: microsoft.graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Н/Д

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|lastUpdateDateTime|Строка|Метка времени последнего обновления.|
|contentNamespaceUrl|Строка|Версия отчета DHA (версия пространства имен).|
|deviceHealthAttestationStatus|Строка|Версия отчета DHA (версия пространства имен).|
|contentVersion|Строка|Версия схемы состояния HealthAttestation.|
|issuedDateTime|DateTimeOffset|Дата и время оценки устройства или его публикации для MDM.|
|attestationIdentityKey|Строка|Если на устройстве имеется ключ удостоверения подлинности (AIK), это свойство указывает на наличие у устройства сертификата ключа подтверждения (EK).|
|resetCount|Int64|Количество переходов компьютера в режим гибернации или возобновлений его работы.|
|restartCount|Int64|Количество перезапусков компьютера.|
|dataExcutionPolicy|Строка|Политика предотвращения выполнения данных (DEP) определяет набор аппаратных и программных технологий, обеспечивающих дополнительные проверки в памяти. |
|bitLockerStatus|Строка|Включение или выключение шифрования диска BitLocker.|
|bootManagerVersion|Строка|Версия диспетчера загрузки.|
|codeIntegrityCheckVersion|Строка|Версия диспетчера загрузки.|
|secureBoot|Строка|Если включена безопасная загрузка, основные компоненты должны включать правильные криптографические подписи.|
|bootDebugging|Строка|Если включено свойство bootDebugging, устройство используется при разработке и тестировании.|
|operatingSystemKernelDebugging|Строка|Если включено свойство operatingSystemKernelDebugging, устройство используется при разработке и тестировании.|
|codeIntegrity|Строка| Если включена целостность кода, выполняется только код, который прошел проверку на целостность.|
|testSigning|Строка|Если разрешена тестовая подпись, устройство не применяет проверку подписи во время загрузки.|
|safeMode|Строка|Безопасный режим — это средство устранения неполадок в Windows, которое запускает компьютер в ограниченном состоянии.|
|windowsPE|Строка|Операционная система, которая запускается с ограниченным набором служб и используется для подготовки компьютера к работе с Windows.|
|earlyLaunchAntiMalwareDriverProtection|Строка|Драйвер ELAM обеспечивает защиту компьютеров в сети при их запуске.|
|virtualSecureMode|Строка|VSM — это контейнер, защищающий ценные ресурсы от компрометации ядра.|
|pcrHashAlgorithm|Строка|Информационный атрибут, определяющий хэш-алгоритм, который использовался доверенным платформенным модулем (TPM).|
|bootAppSecurityVersion|Строка|Номер версии системы безопасности для приложения загрузки.|
|bootManagerSecurityVersion|Строка|Номер версии системы безопасности для приложения загрузки.|
|tpmVersion|Строка|Номер версии системы безопасности для приложения загрузки.|
|pcr0|Строка|Измерение, которое записывается в реестр конфигурации платформы (PCR).\[0\]|
|secureBootConfigurationPolicyFingerPrint|Строка|Отпечаток пользовательской политики настройки безопасной загрузки.|
|codeIntegrityPolicy|Строка|Политика целостности кода, которая управляет безопасностью среды загрузки.|
|bootRevisionListInfo|Строка|Список проверок при загрузке, загруженный во время начальной загрузки на аттестированном устройстве.|
|operatingSystemRevListInfo|Строка|Список проверок операционной системы, загруженный во время начальной загрузки на аттестированном устройстве.|
|healthStatusMismatchInfo|String|Этот атрибут отображается, когда служба DHA обнаруживает ошибку целостности данных.|
|healthAttestationSupportedStatus|String|Этот атрибут указывает, поддерживается ли DHA для устройства.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceHealthAttestationState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceHealthAttestationState",
  "lastUpdateDateTime": "String",
  "contentNamespaceUrl": "String",
  "deviceHealthAttestationStatus": "String",
  "contentVersion": "String",
  "issuedDateTime": "String (timestamp)",
  "attestationIdentityKey": "String",
  "resetCount": 1024,
  "restartCount": 1024,
  "dataExcutionPolicy": "String",
  "bitLockerStatus": "String",
  "bootManagerVersion": "String",
  "codeIntegrityCheckVersion": "String",
  "secureBoot": "String",
  "bootDebugging": "String",
  "operatingSystemKernelDebugging": "String",
  "codeIntegrity": "String",
  "testSigning": "String",
  "safeMode": "String",
  "windowsPE": "String",
  "earlyLaunchAntiMalwareDriverProtection": "String",
  "virtualSecureMode": "String",
  "pcrHashAlgorithm": "String",
  "bootAppSecurityVersion": "String",
  "bootManagerSecurityVersion": "String",
  "tpmVersion": "String",
  "pcr0": "String",
  "secureBootConfigurationPolicyFingerPrint": "String",
  "codeIntegrityPolicy": "String",
  "bootRevisionListInfo": "String",
  "operatingSystemRevListInfo": "String",
  "healthStatusMismatchInfo": "String",
  "healthAttestationSupportedStatus": "String"
}
```




