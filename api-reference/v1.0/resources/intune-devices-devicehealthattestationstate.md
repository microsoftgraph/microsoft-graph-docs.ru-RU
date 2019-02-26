---
title: Тип ресурса deviceHealthAttestationState
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 53fa5cdafdc125fdc32ef599a625c58e3bcbe687
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30256149"
---
# <a name="devicehealthattestationstate-resource-type"></a>Тип ресурса deviceHealthAttestationState

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

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



