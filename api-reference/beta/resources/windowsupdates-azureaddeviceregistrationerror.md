---
title: тип ресурса azureADDeviceRegistrationError
description: Ошибка в процессе регистрации устройства Azure AD, которая не позволяет службе зачислить устройство в управление обновлениями или развернуть контент на устройстве.
author: aarononeal
ms.localizationpriority: medium
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: cd2699c4fecb694e5678d192d07c0fe2f904ee92
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2022
ms.locfileid: "61863524"
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

