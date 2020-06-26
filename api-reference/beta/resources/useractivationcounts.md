---
title: Тип ресурса Усерактиватионкаунтс
description: Ниже указано представление ресурса в формате JSON.
author: krbain
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 6433c1680630b5805cd18a22e550e58a51bcefbc
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/26/2020
ms.locfileid: "44898305"
---
# <a name="useractivationcounts-resource-type"></a>Тип ресурса Усерактиватионкаунтс

Пространство имен: microsoft.graph

## <a name="properties"></a>Свойства

| Свойство          | Тип   | Описание                              |
| :---------------- | :----- | ---------------------------------------- |
| продукттипе       | String | Тип продукта, например "Microsoft 365 профессиональный плюс" или "клиент Project". |
| ластактиватеддате | Дата   | Дата последней активации.       |
| под           | Int64  | Счетчик активаций в Windows. Это число включает все активации на любом компьютере с Windows. |
| mac               | Int64  | Число активаций в Mac OS.          |
| windows10Mobile   | Int64  | Счетчик активаций для Windows 10 Mobile. |
| модуле               | Int64  | Счетчик активаций на iOS.             |
| ОС           | Int64  | Счетчик активаций на устройстве с Android.  |
| активатедоншаредкомпутер   | Boolean | Имеет значение true, если пользователь использовал продукт на общедоступном компьютере. |

## <a name="json-representation"></a>Представление в формате JSON

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
