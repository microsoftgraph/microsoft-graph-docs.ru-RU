---
title: тип ресурса userActivationCounts
description: Ниже указано представление ресурса в формате JSON.
author: jpettere
localization_priority: Normal
ms.prod: users
doc_type: resourcePageType
ms.openlocfilehash: 48adb73bac65ddced88aea3edb18deae7653f5b3
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761795"
---
# <a name="useractivationcounts-resource-type"></a>тип ресурса userActivationCounts

Пространство имен: microsoft.graph

## <a name="properties"></a>Свойства

| Свойство          | Тип   | Описание                              |
| :---------------- | :----- | ---------------------------------------- |
| productType       | String | Тип продукта, например "Microsoft 365 ProPlus" или "Project Client". |
| lastActivatedDate | Дата   | Дата последней активации.       |
| Windows           | Int64  | Активация рассчитывается на Windows. Этот номер включает каждую активацию на любом компьютере Windows. |
| mac               | Int64  | Активация рассчитывается на ОС Mac.          |
| windows10Mobile   | Int64  | Активация рассчитывается на windows 10 mobile. |
| ios               | Int64  | Активация рассчитывается на iOS.             |
| Android           | Int64  | Активация рассчитывается на устройстве Android.  |
| activatedOnSharedComputer   | Boolean | True, если пользователь использовал продукт на общем компьютере раньше. |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.userActivationCounts"
} -->

```json
{
  "productType": "String", 
  "lastActivatedDate": "Date", 
  "windows": 1024, 
  "mac": 1024, 
  "windows10Mobile": 1024, 
  "ios": 1024, 
  "android": 1024,
  "activatedOnSharedComputer": true 
}
```


