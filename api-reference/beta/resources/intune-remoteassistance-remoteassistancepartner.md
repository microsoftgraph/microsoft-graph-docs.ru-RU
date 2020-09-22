---
title: Тип ресурса remoteAssistancePartner
description: Ресурсы Ремотеассистпартнер представляют метаданные и состояние данной службы партнерской службы удаленного помощника.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a28060cbab7510d761d4d0106ac6c965276762df
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48039470"
---
# <a name="remoteassistancepartner-resource-type"></a>Тип ресурса remoteAssistancePartner

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Ресурсы Ремотеассистпартнер представляют метаданные и состояние данной службы партнерской службы удаленного помощника.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список объектов remoteAssistancePartner](../api/intune-remoteassistance-remoteassistancepartner-list.md)|Коллекция [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md)|Список свойств и связей объектов [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md).|
|[Получение объекта remoteAssistancePartner](../api/intune-remoteassistance-remoteassistancepartner-get.md)|[remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md)|Чтение свойств и связей объекта [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md).|
|[Создание объекта remoteAssistancePartner](../api/intune-remoteassistance-remoteassistancepartner-create.md)|[remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md)|Создание объекта [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md).|
|[Удаление объекта remoteAssistancePartner](../api/intune-remoteassistance-remoteassistancepartner-delete.md)|Нет|Удаляет объект [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md).|
|[Обновление объекта remoteAssistancePartner](../api/intune-remoteassistance-remoteassistancepartner-update.md)|[remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md)|Обновление свойств объекта [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md).|
|[Действие beginOnboarding](../api/intune-remoteassistance-remoteassistancepartner-beginonboarding.md)|Нет|Запрос на запуск входящей миграции.  Должен быть связан с соответствующими сведениями учетной записи TeamViewer|
|[Действие disconnect](../api/intune-remoteassistance-remoteassistancepartner-disconnect.md)|Нет|Запрос на удаление активного соединителя TeamViewer Connector|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор партнера.|
|displayName|String|Отображаемое имя партнера.|
|onboardingUrl|String|URL-адрес портала подключения партнера, где администратор может настроить свою службу удаленного помощника.|
|onboardingStatus|[ремотеассистанцеонбоардингстатус](../resources/intune-remoteassistance-remoteassistanceonboardingstatus.md)|Понятное описание состояния текущего соединителя TeamViewer. Возможные значения: `notOnboarded`, `onboarding`, `onboarded`.|
|lastConnectionDateTime|DateTimeOffset|Метка времени последнего запроса, отправленного в службу Intune партнером TEM.|
|онбоардингрекуестекспиридатетиме|DateTimeOffset|Когда свойства onboardingstatus является входящей миграцией, это дата и время истечения срока действия запроса на приподключение.|

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
  "lastConnectionDateTime": "String (timestamp)",
  "onboardingRequestExpiryDateTime": "String (timestamp)"
}
```






