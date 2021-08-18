---
title: Тип ресурса remoteAssistancePartner
description: Ресурсы RemoteAssistPartner представляют метаданные и состояние данной службы партнеров удаленной помощи.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4888ea507e17b962fed9c05dabf722c3c9d1b76dea1af36d78f211d2d6ef5867
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54249771"
---
# <a name="remoteassistancepartner-resource-type"></a>Тип ресурса remoteAssistancePartner

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Ресурсы RemoteAssistPartner представляют метаданные и состояние данной службы партнеров удаленной помощи.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список объектов remoteAssistancePartner](../api/intune-remoteassistance-remoteassistancepartner-list.md)|Коллекция [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md)|Список свойств и связей объектов [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md).|
|[Получение объекта remoteAssistancePartner](../api/intune-remoteassistance-remoteassistancepartner-get.md)|[remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md)|Чтение свойств и связей объекта [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md).|
|[Создание объекта remoteAssistancePartner](../api/intune-remoteassistance-remoteassistancepartner-create.md)|[remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md)|Создание объекта [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md).|
|[Удаление объекта remoteAssistancePartner](../api/intune-remoteassistance-remoteassistancepartner-delete.md)|Нет|Удаляет объект [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md).|
|[Обновление объекта remoteAssistancePartner](../api/intune-remoteassistance-remoteassistancepartner-update.md)|[remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md)|Обновление свойств объекта [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md).|
|[Действие beginOnboarding](../api/intune-remoteassistance-remoteassistancepartner-beginonboarding.md)|Нет|Запрос на запуск бортового.  Должна быть соединая с соответствующими сведениями учетной записи TeamViewer|
|[Действие disconnect](../api/intune-remoteassistance-remoteassistancepartner-disconnect.md)|Нет|Запрос на удаление активного соединиттеля TeamViewer|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор партнера.|
|displayName|Строка|Отображаемое имя партнера.|
|onboardingUrl|String|URL-адрес портала подключения партнера, где администратор может настроить свою службу удаленного помощника.|
|onboardingStatus|[remoteAssistanceOnboardingStatus](../resources/intune-remoteassistance-remoteassistanceonboardingstatus.md)|Удобное описание текущего состояния соединиттеля TeamViewer. Возможные значения: `notOnboarded`, `onboarding`, `onboarded`.|
|lastConnectionDateTime|DateTimeOffset|Метка времени последнего запроса, отправленного в службу Intune партнером TEM.|
|onboardingRequestExpiryDateTime|DateTimeOffset|Когда onboardingStatus находится на борту, это время даты, когда истекает срок действия запроса на борт.|

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
  "lastConnectionDateTime": "String (timestamp)",
  "onboardingRequestExpiryDateTime": "String (timestamp)"
}
```




