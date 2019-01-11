---
title: Тип ресурса userActivationCounts
description: Ниже указано представление ресурса в формате JSON.
author: dkershaw10
localization_priority: Normal
ms.openlocfilehash: cae194545f13d312ee78b572659017752e43a6a6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27845292"
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
