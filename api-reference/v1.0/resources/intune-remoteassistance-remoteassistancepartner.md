---
title: Тип ресурса remoteAssistancePartner
description: Ресурсы remoteAssistPartner представляются метаданные и состояние определенной партнерской службы удаленного помощника.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0557eb45fb770c257f1734bf967f78e9e00cac81
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32554201"
---
# <a name="remoteassistancepartner-resource-type"></a>Тип ресурса remoteAssistancePartner

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

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
|onboardingStatus|[Ремотеассистанцеонбоардингстатус](../resources/intune-remoteassistance-remoteassistanceonboardingstatus.md)|Подлежит определению. Возможные значения: `notOnboarded`, `onboarding`, `onboarded`.|
|lastConnectionDateTime|DateTimeOffset|Метка времени последнего запроса, отправленного службе Intune партнером TEM.|

## <a name="relationships"></a>Отношения
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



