---
title: тип ресурса userActivationCounts
description: Ниже указано представление ресурса в формате JSON.
author: jpettere
ms.localizationpriority: medium
ms.prod: users
doc_type: resourcePageType
ms.openlocfilehash: 466ccc3f942bec2fbb09e094e7805c4fcf160e54
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59033170"
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


