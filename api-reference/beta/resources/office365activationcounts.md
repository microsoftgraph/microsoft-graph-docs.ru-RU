---
title: Тип ресурса office365ActivationCounts
description: Ниже указано представление ресурса в формате JSON.
ms.openlocfilehash: e53a979ac627735ef63a24e1823d83f4c9fe9f7a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27081428"
---
# <a name="office365activationcounts-resource-type"></a>Тип ресурса office365ActivationCounts

## <a name="properties"></a>Свойства

| Свойство          | Тип   | Description                              |
| :---------------- | :----- | ---------------------------------------- |
| reportRefreshDate | Date   | Последняя дата контента.          |
| productType       | String | Тип продукта, например «Office 365 профессиональный плюс», «Клиента Project» или «Visio Pro для Office 365". |
| Windows           | Int64  | Число активации в Windows. Эта цифра включает в себя каждые активации на компьютерах под управлением Windows. |
| mac               | Int64  | Число активации на Mac OS.          |
| Android (en)           | Int64  | Число активации на устройстве Android.  |
| операций ввода-вывода               | Int64  | Число активации на операций ввода-вывода.             |
| windows10Mobile   | Int64  | Активация на количество Windows 10 mobile. |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.office365ActivationCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "productType": "String", 
  "windows": 1024, 
  "mac": 1024, 
  "android": 1024, 
  "ios": 1024, 
  "windows10Mobile": 1024
}
```
