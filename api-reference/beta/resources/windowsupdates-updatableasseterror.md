---
title: тип ресурса updatableAssetError
description: Абстрактный тип, представляюющий ошибку, которая не позволяет службе развертывания зачислить azureADDevice в управление обновлениями или развернуть контент на устройстве
author: aarononeal
ms.localizationpriority: medium
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: 2d90c167f3d2d1ba1033b082be1c534460622bf0
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2022
ms.locfileid: "61792178"
---
# <a name="updatableasseterror-resource-type"></a>тип ресурса updatableAssetError

Пространство имен: microsoft.graph.windowsUpdates

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Абстрактный тип, представляюющий ошибку, которая не позволяет службе развертывания зачислить [azureADDevice](../resources/windowsupdates-azureaddevice.md) в управление обновлениями или развернуть содержимое на устройстве. 

Все updatable ошибки активов имеют производный [тип, azureADDeviceRegistrationError](../resources/windowsupdates-azureaddeviceregistrationerror.md).


## <a name="properties"></a>Свойства
Нет

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsUpdates.updatableAssetError"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.updatableAssetError"
}
```

