---
title: тип ресурса userActivationCounts
description: Ниже указано представление ресурса в формате JSON.
author: jpettere
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 719a73739a64dca2bd7a052cc9cdd51007173eff
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50719901"
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


