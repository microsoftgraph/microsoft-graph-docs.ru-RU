---
title: Тип ресурса Усерактиватионкаунтс
description: Ниже указано представление ресурса в формате JSON.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 535355d6be3f6b617d7eb293890aa05a517cfc3b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32581284"
---
# <a name="useractivationcounts-resource-type"></a>Тип ресурса Усерактиватионкаунтс

## <a name="properties"></a>Свойства

| Свойство          | Тип   | Описание                              |
| :---------------- | :----- | ---------------------------------------- |
| Продукттипе       | String | Тип продукта, например "Office 365 профессиональный плюс", "клиент Project" или "Visio Pro для Office 365". |
| Ластактиватеддате | Дата   | Дата последней активации.       |
| под           | Int64  | Счетчик активаций в Windows. Это число включает все активации на любом компьютере с Windows. |
| mac               | Int64  | Число активаций в Mac OS.          |
| windows10Mobile   | Int64  | Счетчик активаций для Windows 10 Mobile. |
| модуле               | Int64  | Счетчик активаций на iOS.             |
| ОС           | Int64  | Счетчик активаций на устройстве с Android.  |
| Активатедоншаредкомпутер   | Boolean | Имеет значение true, если пользователь использовал продукт на общедоступном компьютере. |

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
