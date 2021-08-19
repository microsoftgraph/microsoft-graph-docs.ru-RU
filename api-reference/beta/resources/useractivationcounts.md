---
title: тип ресурса userActivationCounts
description: Ниже указано представление ресурса в формате JSON.
author: jpettere
localization_priority: Normal
ms.prod: users
doc_type: resourcePageType
ms.openlocfilehash: 9e1783822daf9ead4ba130161976c2f65f4c74a2f8b0f8a828981b14e64bcdf9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54212831"
---
# <a name="useractivationcounts-resource-type"></a>тип ресурса userActivationCounts

Пространство имен: microsoft.graph

## <a name="properties"></a>Свойства

| Свойство          | Тип   | Описание                              |
| :---------------- | :----- | ---------------------------------------- |
| productType       | Строка | Тип продукта, например "Microsoft 365 ProPlus" или "Project клиент". |
| lastActivatedDate | Дата   | Дата последней активации.       |
| Windows           | Int64  | Активация рассчитывается на Windows. Этот номер включает каждую активацию на любом Windows компьютере. |
| mac               | Int64  | Активация рассчитывается на ОС Mac.          |
| windows10Mobile   | Int64  | Активация рассчитывается на Windows 10 мобильном телефоне. |
| ios               | Int64  | Активация рассчитывается на iOS.             |
| Android           | Int64  | Активация рассчитывается на устройстве Android.  |
| activatedOnSharedComputer   | Логический | True, если пользователь использовал продукт на общем компьютере раньше. |

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


