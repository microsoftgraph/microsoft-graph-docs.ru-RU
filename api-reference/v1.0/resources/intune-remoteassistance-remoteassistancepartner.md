---
title: Тип ресурса remoteAssistancePartner
description: Ресурсы remoteAssistPartner представляются метаданные и состояние определенной партнерской службы удаленного помощника.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 9eca68f2a2feb2906f1d2b55b3f857d515a22c50
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43441559"
---
# <a name="remoteassistancepartner-resource-type"></a>Тип ресурса remoteAssistancePartner

Пространство имен: microsoft.graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Ресурсы remoteAssistPartner представляются метаданные и состояние определенной партнерской службы удаленного помощника.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список объектов remoteAssistancePartner](../api/intune-remoteassistance-remoteassistancepartner-list.md)|Коллекция [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md)|Список свойств и связей объектов [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md).|
|[Получение объекта remoteAssistancePartner](../api/intune-remoteassistance-remoteassistancepartner-get.md)|[remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md)|Чтение свойств и связей объекта [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md).|
|[Создание объекта remoteAssistancePartner](../api/intune-remoteassistance-remoteassistancepartner-create.md)|[remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md)|Создание объекта [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md).|
|[Удаление объекта remoteAssistancePartner](../api/intune-remoteassistance-remoteassistancepartner-delete.md)|Нет|Удаляет объект [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md).|
|[Обновление объекта remoteAssistancePartner](../api/intune-remoteassistance-remoteassistancepartner-update.md)|[remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md)|Обновление свойств объекта [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md).|
|[Действие beginOnboarding](../api/intune-remoteassistance-remoteassistancepartner-beginonboarding.md)|None|Н/Д|
|[Действие disconnect](../api/intune-remoteassistance-remoteassistancepartner-disconnect.md)|Нет|Пока не задокументировано|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор партнера.|
|displayName|Строка|Отображаемое имя партнера.|
|onboardingUrl|String|URL-адрес портала подключения партнера, где администратор может настроить свою службу удаленного помощника.|
|onboardingStatus|[ремотеассистанцеонбоардингстатус](../resources/intune-remoteassistance-remoteassistanceonboardingstatus.md)|Подлежит определению. Возможные значения: `notOnboarded`, `onboarding`, `onboarded`.|
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







