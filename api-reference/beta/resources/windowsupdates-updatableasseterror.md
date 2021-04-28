---
title: тип ресурса updatableAssetError
description: Абстрактный тип, представляюющий ошибку, которая не позволяет службе развертывания зачислить azureADDevice в управление обновлениями или развернуть контент на устройстве
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: 4d4375be68aea6dd4cb27c7ae8b78aaf86a2edf1
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067499"
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

