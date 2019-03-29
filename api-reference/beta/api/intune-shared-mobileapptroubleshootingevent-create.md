---
title: Создание Мобилеапптраублешутинжевент
description: Описывает метод Create Мобилеапптраублешутинжевент API Microsoft Graph для Intune, который поддерживает несколько рабочих процессов.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 89a191f94d68636226b6a8d41be0d9ba962da761
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30979265"
---
# <a name="create-mobileapptroubleshootingevent"></a>Создание Мобилеапптраублешутинжевент

> **Важно!** API в версии/Beta в Microsoft Graph могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Создание нового объекта [мобилеапптраублешутинжевент](../resources/intune-shared-mobileapptroubleshootingevent.md) .

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке убывания привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)||
|&nbsp; &nbsp; **Управление устройствами**|DeviceManagementManagedDevices.ReadWrite.All|
|&nbsp; &nbsp; **Устранение неполадок**|DeviceManagementManagedDevices.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|Не поддерживается.|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/mobileAppTroubleshootingEvents
POST /users/{usersId}/mobileAppTroubleshootingEvents
```

## <a name="request-headers"></a>Заголовки запросов
|Заголовок|Значение|
|:---|:---|
|Авторизация|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В тексте запроса добавьте представление объекта Мобилеапптраублешутинжевент в формате JSON.

В следующей таблице приведены свойства, необходимые при создании Мобилеапптраублешутинжевент.

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|GUID объекта|
|**Устранение неполадок**|
|Аддитионалинформатион|Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)|Набор пар строкового ключа и строкового значения, предоставляющий дополнительные сведения о событии устранения неполадок.|
|applicationId|String|Идентификатор приложения Intune.|
|correlationId|String|Идентификатор, используемый для трассировки сбоя в службе. |
|eventDateTime|DateTimeOffset|Время возникновения события. |
|eventName|String|Имя события, соответствующее соБытию устранения неполадок. Необязательное свойство.|
|лист|Коллекция [мобилеапптраублешутингхисторитем](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)|Элемент журнала устранения неполадок мобильных приложений Intune|
|managedDeviceIdentifier|String|Идентификатор события, созданный или полученный службой Intune.|
|Траублешутинжеррордетаилс|[deviceManagementTroubleshootingErrorDetails](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|Объект, содержащий подробные сведения об ошибке и ее исправлении. |
|userId|String|Идентификатор пользователя, который пытался зарегистрировать устройство.|

## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [мобилеапптраублешутинжевент](../resources/intune-shared-mobileapptroubleshootingevent.md) в тексте отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/mobileAppTroubleshootingEvents
Content-type: application/json
Content-length: 71

{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingEvent"
}
```

### <a name="response"></a>Отклик
Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 120

{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingEvent",
  "id": "77943c10-3c10-7794-103c-9477103c9477"
}
```




