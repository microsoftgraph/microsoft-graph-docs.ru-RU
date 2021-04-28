---
title: тип ресурса azureADDeviceRegistrationError
description: Ошибка в процессе регистрации устройства Azure AD, которая не позволяет службе зачислить устройство в управление обновлениями или развернуть контент на устройстве.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: 1d08ab96d5298c70f34acf89e3c6c4605d9df0a1
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/28/2021
ms.locfileid: "52068117"
---
# <a name="azureaddeviceregistrationerror-resource-type"></a>тип ресурса azureADDeviceRegistrationError

Пространство имен: microsoft.graph.windowsUpdates

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ошибка в процессе регистрации устройства [Azure AD,](../resources/windowsupdates-azureaddevice.md) которая не позволяет службе зачислить устройство в управление обновлениями или развернуть контент на устройстве.

Наследует [от updatableAssetError](../resources/windowsupdates-updatableasseterror.md).

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|reason|microsoft.graph.windowsUpdates.azureADDeviceRegistrationErrorReason|Причина, по которой регистрация столкнулась с ошибкой. Возможные значения: `invalidGlobalDeviceId`, `invalidAzureADDeviceId`, `missingTrustType`, `invalidAzureADJoin`.|

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

