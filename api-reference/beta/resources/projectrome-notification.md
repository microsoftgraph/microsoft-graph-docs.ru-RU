---
title: Тип ресурса notification
description: 'Представляет уведомление, опубликованного сервером приложений, которое ориентировано на указанного пользователя. Уведомление хранится в Microsoft Graph и распространяется на разные конечные точки устройств, владельцем которые является пользователь. '
localization_priority: Normal
ms.prod: notifications
doc_type: resourcePageType
author: merzink
ms.openlocfilehash: abd17119e80e4e8a7967197356811ee519d813ba
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50159453"
---
# <a name="notification-resource-type"></a>Тип ресурса notification

Пространство имен: microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет уведомление, опубликованного сервером приложений, которое ориентировано на указанного пользователя. Уведомление хранится в Microsoft Graph и распространяется на разные конечные точки устройств, владельцем которые является пользователь. 

Уведомление может быть полезной нагрузкой визуального уведомления, которая может интерпретироваться операционной системой (платформы Windows, Android и iOS). Это также может быть полезной нагрузкой данных (rawContent), которая доставляется и обрабатывается клиентами приложений (в том числе через Интернет), которые затем определяют соответствующий пользовательский интерфейс на каждом устройстве.  Обычно это визуальный пользовательский интерфейс уведомления, созданный локально, соответствующий содержимому в исходных данных. 

Когда пользователь работает с визуальным уведомлением, клиент приложения может использовать клиентский SDK уведомлений для обновления состояния соответствующего канала уведомлений в Microsoft Graph, например, пометив уведомление как отклоненное. Затем обновление распространяется на все остальные конечные точки клиента приложения, и клиенты обрабатывают изменение соответствующим образом, например, замещение уведомления, чтобы пользователь не видел избыточные сведения. Клиенты приложений могут получить доступ к одному ресурсу уведомлений позже, прежде чем он истечет (даже после его пометки как отклоненный) в качестве истории уведомлений через [SDK уведомлений.](https://aka.ms/GNSDK) 

> [!NOTE]
> Обновления состояния уведомлений, такие как чтение или отклонение, не будут развещены на веб-конечных точках. Это необходимо, поскольку для веб-push-уведомлений в различных браузерах пользователю требуются визуальные всплывающие уведомления. Поскольку изменения состояния не имеют соответствующего визуального содержимого, они будут развещены только для уведомлений, нацеленных на платформы Windows, iOS или Android.

## <a name="methods"></a>Методы
|Метод | Возвращаемый тип | Описание|
|:------|:------------|:-----------|
|[Создание уведомления](../api/user-post-notifications.md) | [notification](projectrome-notification.md) |Создание и отправка уведомления. |

## <a name="properties"></a>Свойства
|Имя | Тип | Описание|
|:----|:-----|:-----------|
| targetHostName | String | Представляет имя хоста приложения, для которого служба звонков хочет опубликовать уведомление для данного пользователя. При нацеливании на конечные точки веб-сайта (см. **targetPolicy.platformTypes),** убедитесь, что **targetHostName** является тем же именем, которое используется при создании подписки на стороне клиента в свойстве JSON приложения. |
| appNotificationId | String | Уникальный ИД, установленный сервером приложений уведомления, используемого для идентификации и определения отдельного уведомления. |
| groupName | String | Имя группы, к которой принадлежит это уведомление. Он устанавливается разработчиком для группировки уведомлений. |
| targetPolicy | [targetPolicyEndpoints](targetpolicyendpoints.md) | Объект целевой политики обрабатывает политику доставки уведомлений для типов конечных точек, которые должны быть целевыми (Windows, iOS, Android и WebPush) для данного пользователя. |
| payload | [payloadTypes](payloadtypes.md)| Это содержимое данных необработанных или визуальных уведомлений пользователя, которые будут доставляться и потребляться клиентом приложения, получившего это уведомление. |
| displayTimeToLive | Int32 | Задает время (в секундах) для этого содержимого уведомлений в представлении уведомлений каждой платформы. Например, когда уведомление доставляется на устройство с Windows, значение этого свойства передается в ToastNotification.ExpirationTime, которое определяет, как долго всплывающее уведомление будет оставаться в центре уведомлений Windows пользователя. |
| expirationDateTime | DateTimeOffset | Задает дату и время окончания срока действия в формате UTC для уведомления пользователя в формате ISO 8601 (например, полночь 1 января 2019 г. в формате UTC выглядит так: `'2019-01-01T00:00:00Z'` ). После того как время работы, уведомление полностью удаляется из веб-канала уведомлений Microsoft Graph и больше не является частью истории уведомлений. Максимальное значение — 30 дней. |
| priority | string | Указывает приоритет необработанных уведомлений пользователя. Визуальные уведомления отправляются с высоким приоритетом по умолчанию. Допустимые значения: `None`, `High` и `Low`. |
| fallbackPolicy | [fallbackpolicy](fallbackpolicy.md) | Необязательный объект политики отката обрабатывает политику отката уведомлений только для конечных точек iOS и предназначен для использования для необработанных уведомлений с высоким приоритетом, которые могут не доставляться на устройства из-за определенных ограничений платформы (например, режима экономии заряда). |


## <a name="relationships"></a>Связи
Отсутствуют.


## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.notification",
  "keyProperty": "id"
}-->

```json
{
  "targetHostName": "String",
  "appNotificationid": "String (identifier)",
  "groupName": "String", 
  "targetPolicy": {"@odata.type": "microsoft.graph.targetPolicyEndpoints"},
  "payload": {"@odata.type": "microsoft.graph.payloadTypes"},
  "displayTimeToLive": 1024,
  "expirationDateTime": "String (timestamp)",
  "priority": "string",
  "fallbackPolicy": {"@odata.type": "microsoft.graph.fallbackpolicy"},  
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "notification resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


