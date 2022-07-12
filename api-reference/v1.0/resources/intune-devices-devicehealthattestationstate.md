---
title: Тип ресурса deviceHealthAttestationState
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c040e0ff3b54c65850b8d2efaa82c5d0146c2f70
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/12/2022
ms.locfileid: "66720726"
---
# <a name="devicehealthattestationstate-resource-type"></a>Тип ресурса deviceHealthAttestationState

Пространство имен: microsoft.graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Н/Д

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|lastUpdateDateTime|String|Метка времени последнего обновления.|
|contentNamespaceUrl|String|Версия отчета DHA (версия пространства имен).|
|deviceHealthAttestationStatus|String|Версия отчета DHA (версия пространства имен).|
|contentVersion|String|Версия схемы состояния HealthAttestation.|
|issuedDateTime|DateTimeOffset|Дата и время оценки устройства или его публикации для MDM.|
|attestationIdentityKey|String|Если на устройстве имеется ключ удостоверения подлинности (AIK), это свойство указывает на наличие у устройства сертификата ключа подтверждения (EK).|
|resetCount|Int64|Количество переходов компьютера в режим гибернации или возобновлений его работы.|
|restartCount|Int64|Количество перезапусков компьютера.|
|dataExcutionPolicy|String|Политика предотвращения выполнения данных (DEP) определяет набор аппаратных и программных технологий, обеспечивающих дополнительные проверки в памяти. |
|bitLockerStatus|String|Включение или выключение шифрования диска BitLocker.|
|bootManagerVersion|String|Версия диспетчера загрузки.|
|codeIntegrityCheckVersion|String|Версия диспетчера загрузки.|
|secureBoot|String|Если включена безопасная загрузка, основные компоненты должны включать правильные криптографические подписи.|
|bootDebugging|String|Если включено свойство bootDebugging, устройство используется при разработке и тестировании.|
|operatingSystemKernelDebugging|String|Если включено свойство operatingSystemKernelDebugging, устройство используется при разработке и тестировании.|
|codeIntegrity|String| Если включена целостность кода, выполняется только код, который прошел проверку на целостность.|
|testSigning|String|Если разрешена тестовая подпись, устройство не применяет проверку подписи во время загрузки.|
|safeMode|String|Безопасный режим — это средство устранения неполадок в Windows, которое запускает компьютер в ограниченном состоянии.|
|windowsPE|String|Операционная система, которая запускается с ограниченным набором служб и используется для подготовки компьютера к работе с Windows.|
|earlyLaunchAntiMalwareDriverProtection|String|Драйвер ELAM обеспечивает защиту компьютеров в сети при их запуске.|
|virtualSecureMode|String|VSM — это контейнер, защищающий ценные ресурсы от компрометации ядра.|
|pcrHashAlgorithm|String|Информационный атрибут, определяющий хэш-алгоритм, который использовался доверенным платформенным модулем (TPM).|
|bootAppSecurityVersion|String|Номер версии системы безопасности для приложения загрузки.|
|bootManagerSecurityVersion|String|Номер версии системы безопасности для приложения загрузки.|
|tpmVersion|String|Номер версии системы безопасности для приложения загрузки.|
|pcr0|String|Измерение, которое записывается в реестр конфигурации платформы (PCR).\[0\]|
|secureBootConfigurationPolicyFingerPrint|String|Отпечаток пользовательской политики настройки безопасной загрузки.|
|codeIntegrityPolicy|String|Политика целостности кода, которая управляет безопасностью среды загрузки.|
|bootRevisionListInfo|String|Список проверок при загрузке, загруженный во время начальной загрузки на аттестированном устройстве.|
|operatingSystemRevListInfo|String|Список проверок операционной системы, загруженный во время начальной загрузки на аттестированном устройстве.|
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





