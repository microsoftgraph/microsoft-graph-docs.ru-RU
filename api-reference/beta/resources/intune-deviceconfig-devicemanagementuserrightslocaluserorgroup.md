---
title: Тип ресурса deviceManagementUserRightsLocalUserOrGroup
description: Представляет сведения для локального пользователя или группы, используемые для настройки прав пользователя.
author: tfitzmac
ms.openlocfilehash: baabd2f3bb9e3bce44d172cd83f61f57c5c2c98d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27303733"
---
# <a name="devicemanagementuserrightslocaluserorgroup-resource-type"></a>Тип ресурса deviceManagementUserRightsLocalUserOrGroup

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Представляет сведения для локального пользователя или группы, используемые для настройки прав пользователя.
## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|name|Строка|Имя этого локального пользователя или группы.|
|описание|Строка|Описание администратора локального пользователя или группы.|
|Класс securityIdentifier|String.|Идентификатор безопасности этого локального пользователя или группы (например * S-1-5-32-544).|

## <a name="relationships"></a>Связи
Нет
## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
  "name": "String",
  "description": "String",
  "securityIdentifier": "String"
}
```





