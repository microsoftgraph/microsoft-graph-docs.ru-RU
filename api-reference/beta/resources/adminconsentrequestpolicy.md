---
title: тип ресурса adminConsentRequestPolicy
description: Указывает политику, с помощью которой можно создавать и управлять запросами на согласие для всего клиента.
author: psignoret
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: dde04ac8c94f0f924df47f3b9490b09f18490c2c
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50965238"
---
# <a name="adminconsentrequestpolicy-resource-type"></a>тип ресурса adminConsentRequestPolicy

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Указывает политику, в которой создаются и управляются запросы на согласие для всего клиента. Существует один **администраторConsentRequestPolicy для** каждого клиента. 

**АдминистраторConsentRequestPolicy** предоставляет дополнительные параметры при создании запроса на согласие, чтобы контролировать поведение функции при запуске запроса на согласие.

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Получить adminConsentRequestPolicy](../api/adminconsentrequestpolicy-get.md)|[adminConsentRequestPolicy](../resources/adminconsentrequestpolicy.md)|Ознакомьтесь с свойствами и отношениями объекта [adminConsentRequestPolicy.](../resources/adminconsentrequestpolicy.md)|
|[Обновление adminConsentRequestPolicy](../api/adminconsentrequestpolicy-update.md)|[adminConsentRequestPolicy](../resources/adminconsentrequestpolicy.md)|Обновление свойств объекта [adminConsentRequestPolicy.](../resources/adminconsentrequestpolicy.md)|


## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|isEnabled|Boolean|Указывает, включена или отключена функция запроса на согласие администратора. Обязательный.|
|notifyReviewers|Boolean|Указывает, будут ли рецензенты получать уведомления. Обязательный.|
|remindersEnabled|Boolean|Указывает, будут ли рецензенты получать сообщения напоминания. Обязательный.|
|requestDurationInDays|Int32|Указывает продолжительность действия запроса до его автоматического истечения, если не будет применено решение.|
|рецензенты|[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) collection|Обязательный.|
|version|Int32|Указывает версию этой политики. Когда политика обновляется, эта версия обновляется. Только для чтения.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.adminConsentRequestPolicy",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.adminConsentRequestPolicy",
  "isEnabled": "Boolean",
  "version": "Integer",
  "notifyReviewers": "Boolean",
  "remindersEnabled": "Boolean",
  "requestDurationInDays": "Integer",
  "reviewers": [
    {
      "@odata.type": "microsoft.graph.accessReviewReviewerScope"
    }
  ]
}
```
