---
title: Тип ресурса userActivationCounts
description: Ниже указано представление ресурса в формате JSON.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 535355d6be3f6b617d7eb293890aa05a517cfc3b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27980351"
---
# <a name="useractivationcounts-resource-type"></a>Тип ресурса userActivationCounts

## <a name="properties"></a>Свойства

| Свойство          | Тип   | Описание                              |
| :---------------- | :----- | ---------------------------------------- |
| productType       | Строка | Тип продукта, например «Office 365 профессиональный плюс», «Клиента Project» или «Visio Pro для Office 365". |
| lastActivatedDate | Date   | Дата последней активации.       |
| Windows           | Int64  | Число активации в Windows. Эта цифра включает в себя каждые активации на компьютерах под управлением Windows. |
| mac               | Int64  | Число активации на Mac OS.          |
| windows10Mobile   | Int64  | Активация на количество Windows 10 mobile. |
| операций ввода-вывода               | Int64  | Число активации на операций ввода-вывода.             |
| Android (en)           | Int64  | Число активации на устройстве Android.  |
| activatedOnSharedComputer   | Логический | Значение true, если пользователь продукта на совместно используемый компьютер перед. |

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
