---
title: Тип ресурса remoteAssistancePartner
description: Ресурсы remoteAssistPartner представляются метаданные и состояние определенной партнерской службы удаленного помощника.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 52badd2ad146f23fba70ab545a459b124e7fae2c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27821716"
---
# <a name="remoteassistancepartner-resource-type"></a>Тип ресурса remoteAssistancePartner

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Ресурсы remoteAssistPartner представляются метаданные и состояние определенной партнерской службы удаленного помощника.
## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список объектов remoteAssistancePartner](../api/intune-remoteassistance-remoteassistancepartner-list.md)|Коллекция [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md)|Список свойств и связей объектов [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md).|
|[Получение объекта remoteAssistancePartner](../api/intune-remoteassistance-remoteassistancepartner-get.md)|[remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md)|Чтение свойств и связей объекта [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md).|
|[Создание объекта remoteAssistancePartner](../api/intune-remoteassistance-remoteassistancepartner-create.md)|[remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md)|Создание объекта [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md).|
|[Удаление объекта remoteAssistancePartner](../api/intune-remoteassistance-remoteassistancepartner-delete.md)|Нет|Удаляет объект [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md).|
|[Обновление объекта remoteAssistancePartner](../api/intune-remoteassistance-remoteassistancepartner-update.md)|[remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md)|Обновление свойств объекта [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md).|
|[Действие beginOnboarding](../api/intune-remoteassistance-remoteassistancepartner-beginonboarding.md)|Нет|Н/Д|
|[Действие disconnect](../api/intune-remoteassistance-remoteassistancepartner-disconnect.md)|Нет|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор партнера.|
|displayName|String|Отображаемое имя партнера.|
|onboardingUrl|String|URL-адрес портала подключения партнера, где администратор может настроить свою службу удаленного помощника.|
|onboardingStatus|[remoteAssistanceOnboardingStatus](../resources/intune-remoteassistance-remoteassistanceonboardingstatus.md)|БУДЕТ ОПРЕДЕЛЕНО ПОЗЖЕ. Возможные значения: `notOnboarded`, `onboarding`, `onboarded`.|
|lastConnectionDateTime|DateTimeOffset|Метка времени последнего запроса, отправленного службе Intune партнером TEM.|

## <a name="relationships"></a>Связи
Нет
## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.remoteAssistancePartner"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.remoteAssistancePartner",
  "id": "String (identifier)",
  "displayName": "String",
  "onboardingUrl": "String",
  "onboardingStatus": "String",
  "lastConnectionDateTime": "String (timestamp)"
}
```





