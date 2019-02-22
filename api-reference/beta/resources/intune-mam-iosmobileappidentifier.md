---
title: Тип ресурса iosMobileAppIdentifier
description: Идентификатор приложения для iOS.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4b62a6d9ca0a864f703ddb41eee4f147098e740a
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30154105"
---
# <a name="iosmobileappidentifier-resource-type"></a>Тип ресурса iosMobileAppIdentifier

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Идентификатор приложения для iOS.


Наследуется от [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|bundleId|String|Идентификатор приложения, указанный в магазине приложений.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosMobileAppIdentifier"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosMobileAppIdentifier",
  "bundleId": "String"
}
```




