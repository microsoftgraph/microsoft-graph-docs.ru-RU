---
title: Тип ресурса userActivationCounts
description: Ниже указано представление ресурса в формате JSON.
author: dkershaw10
ms.openlocfilehash: 396f6182d000df6d701e8c0cbad3dd02a258c4c0
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27322920"
---
# <a name="useractivationcounts-resource-type"></a>Тип ресурса userActivationCounts

## <a name="properties"></a>Свойства

| Свойство          | Тип   | Описание                              |
| :---------------- | :----- | ---------------------------------------- |
| productType       | String. | Тип продукта, например «Office 365 профессиональный плюс», «Клиента Project» или «Visio Pro для Office 365". |
| lastActivatedDate | Date   | Дата последней активации.       |
| Windows           | Int64  | Число активации в Windows. Эта цифра включает в себя каждые активации на компьютерах под управлением Windows. |
| mac               | Int64  | Число активации на Mac OS.          |
| windows10Mobile   | Int64  | Активация на количество Windows 10 mobile. |
| операций ввода-вывода               | Int64  | Число активации на операций ввода-вывода.             |
| Android (en)           | Int64  | Число активации на устройстве Android.  |
| activatedOnSharedComputer   | Boolean. | Значение true, если пользователь продукта на совместно используемый компьютер перед. |

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
