---
title: Тип ресурса userActivationCounts
description: Ниже указано представление ресурса в формате JSON.
ms.openlocfilehash: 022b73310a54877889efebabbb6e8fc4ab71fb65
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27077807"
---
# <a name="useractivationcounts-resource-type"></a>Тип ресурса userActivationCounts

## <a name="properties"></a>Свойства

| Свойство          | Тип   | Description                              |
| :---------------- | :----- | ---------------------------------------- |
| productType       | String | Тип продукта, например «Office 365 профессиональный плюс», «Клиента Project» или «Visio Pro для Office 365". |
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
