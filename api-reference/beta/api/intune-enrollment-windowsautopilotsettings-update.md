---
title: Обновление windowsAutopilotSettings
description: Обновление свойства объекта windowsAutopilotSettings.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: a0c7f0fba63fa94bfdf2d5a6f9eebd344aa12b93
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29394252"
---
# <a name="update-windowsautopilotsettings"></a>Обновление windowsAutopilotSettings

> **Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Обновление свойства объекта [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) .

## <a name="prerequisites"></a>Предварительные требования
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).

|Тип разрешения|Разрешения (в порядке убывания привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementServiceConfig.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|Не поддерживается.|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsAutopilotSettings
```

## <a name="request-headers"></a>Заголовки запросов
|Заголовок|Значение|
|:---|:---|
|Authorization|Требуется Bearer &lt;маркер&gt;
|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В тексте запроса укажите представление JSON для объекта [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) .

В следующей таблице показаны свойства, которые необходимы для создания [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md).

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|GUID объекта|
|lastSyncDateTime|DateTimeOffset|Последней полной синхронизации даты-времени со службой набору доменов Обнаружения.|
|lastManualSyncTriggerDateTime|DateTimeOffset|Последней полной синхронизации даты-времени со службой набору доменов Обнаружения.|
|syncStatus|[windowsAutopilotSyncStatus](../resources/intune-enrollment-windowsautopilotsyncstatus.md)|Указывает состояние синхронизации со службой синхронизации (набору доменов Обнаружения) данных устройства. Возможные значения: `unknown`, `inProgress`, `completed`, `failed`.|



## <a name="response"></a>Отклик
Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) объекта в теле ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotSettings
Content-type: application/json
Content-length: 230

{
  "@odata.type": "#microsoft.graph.windowsAutopilotSettings",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "lastManualSyncTriggerDateTime": "2016-12-31T23:57:54.7364636-08:00",
  "syncStatus": "inProgress"
}
```

### <a name="response"></a>Отклик
Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 279

{
  "@odata.type": "#microsoft.graph.windowsAutopilotSettings",
  "id": "08c16770-6770-08c1-7067-c1087067c108",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "lastManualSyncTriggerDateTime": "2016-12-31T23:57:54.7364636-08:00",
  "syncStatus": "inProgress"
}
```




