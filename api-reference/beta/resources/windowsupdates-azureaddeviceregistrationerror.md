---
title: тип ресурса azureADDeviceRegistrationError
description: Ошибка в процессе регистрации устройства Azure AD, которая не позволяет службе зачислить устройство в управление обновлениями или развернуть контент на устройстве.
author: Alice-at-Microsoft
ms.localizationpriority: medium
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: 8ef1d16203f4b2197a0f8cdb93aaeae073d77ccb
ms.sourcegitcommit: c6a8c1cc13ace38d6c4371139ee84707c5c93352
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2021
ms.locfileid: "60890369"
---
# <a name="azureaddeviceregistrationerror-resource-type"></a>тип ресурса azureADDeviceRegistrationError

Пространство имен: microsoft.graph.windowsUpdates

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ошибка в процессе регистрации устройства [Azure AD,](../resources/windowsupdates-azureaddevice.md) которая не позволяет службе зачислить устройство в управление обновлениями или развернуть контент на устройстве.

Наследует [от updatableAssetError](../resources/windowsupdates-updatableasseterror.md).

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|reason|microsoft.graph.windowsUpdates.azureADDeviceRegistrationErrorReason|Причина, по которой регистрация столкнулась с ошибкой. Возможные значения: `invalidGlobalDeviceId`, `invalidAzureADDeviceId`, `missingTrustType`, `invalidAzureADJoin`, `unknownFutureValue`.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsUpdates.azureADDeviceRegistrationError"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.azureADDeviceRegistrationError",
  "reason": "String"
}
```

