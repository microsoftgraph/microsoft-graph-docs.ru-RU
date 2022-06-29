---
title: Обновление mobileAppTroubleshootingEvent
description: Описывает метод Update mobileAppTroubleshootingEvent microsoft API Graph for Intune, который поддерживает несколько рабочих процессов.
localization_priority: Normal
author: dougeby
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0d54bdc17e2965d0f69a9588c6d30e48a86eea59
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/29/2022
ms.locfileid: "66447284"
---
# <a name="update-mobileapptroubleshootingevent"></a>Обновление mobileAppTroubleshootingEvent

Пространство имен: microsoft.graph

> **Важно:** API-интерфейсы в версии /beta в Microsoft Graph могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Обновление свойств объекта [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) .

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке убывания привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)||
|&nbsp; &nbsp; **Управление устройствами**|DeviceManagementManagedDevices.ReadWrite.All|
|&nbsp; &nbsp; **Устранение неполадок**|DeviceManagementManagedDevices.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Приложение||
|&nbsp; &nbsp; **Управление устройствами**|DeviceManagementManagedDevices.ReadWrite.All|
|&nbsp; &nbsp; **Устранение неполадок**|DeviceManagementManagedDevices.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
PATCH /users/{usersId}/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Авторизация|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В тексте запроса добавьте представление объекта [mobileAppTroubleshootingEvent в формате](../resources/intune-shared-mobileapptroubleshootingevent.md) JSON.

В следующей таблице показаны свойства, необходимые при создании [объекта mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md).

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|GUID объекта|
|**Устранение неполадок**|
|additionalInformation|Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)|Набор пар строкового ключа и строкового значения, который предоставляет дополнительные сведения о событии устранения неполадок.|
|applicationId|String|Intune идентификатор приложения.|
|correlationId|String|Идентификатор, используемый для трассировки сбоя в службе. |
|eventDateTime|DateTimeOffset|Время возникновения события. |
|eventName|String|Имя события, соответствующее событию устранения неполадок. Необязательное свойство.|
|Истории|[Коллекция mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)|Intune журнала устранения неполадок мобильного приложения.|
|managedDeviceIdentifier|String|Идентификатор события, созданный или полученный службой Intune.|
|troubleshootingErrorDetails|[deviceManagementTroubleshootingErrorDetails](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|Объект, содержащий подробные сведения об ошибке и ее исправлении. |
|userId|String|Идентификатор пользователя, который пытался зарегистрировать устройство.|

## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает код `200 OK` отклика и обновленный объект [mobileAppTroubleshootingEvent](../resources/intune-shared-mobileapptroubleshootingevent.md) в тексте отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}
Content-type: application/json
Content-length: 71

{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingEvent"
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 120

{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingEvent",
  "id": "77943c10-3c10-7794-103c-9477103c9477"
}
```










