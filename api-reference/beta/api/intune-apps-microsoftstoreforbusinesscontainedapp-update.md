---
title: Обновление Микрософтсторефорбусинессконтаинедапп
description: Обновление свойств объекта Микрософтсторефорбусинессконтаинедапп.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3a25ce46c353902feb700bdf1a853d3998f34eee
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42450848"
---
# <a name="update-microsoftstoreforbusinesscontainedapp"></a>Обновление Микрософтсторефорбусинессконтаинедапп

Пространство имен: Microsoft. Graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Обновление свойств объекта [микрософтсторефорбусинессконтаинедапп](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) .

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке убывания привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementApps.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|DeviceManagementApps.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps/{mobileContainedAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.microsoftStoreForBusinessApp/containedApps/{mobileContainedAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.windowsUniversalAppX/committedContainedApps/{mobileContainedAppId}
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Authorization|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В тексте запроса добавьте представление объекта [микрософтсторефорбусинессконтаинедапп](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) в формате JSON.

В следующей таблице приведены свойства, необходимые при создании [микрософтсторефорбусинессконтаинедапп](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md).

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта. Наследуется от [мобилеконтаинедапп](../resources/intune-apps-mobilecontainedapp.md)|
|Модели|String|ИДЕНТИФИКАТОР пользовательской модели приложения для вложенного приложения MicrosoftStoreForBusinessApp.|



## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [микрософтсторефорбусинессконтаинедапп](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) в тексте отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps/{mobileContainedAppId}
Content-type: application/json
Content-length: 127

{
  "@odata.type": "#microsoft.graph.microsoftStoreForBusinessContainedApp",
  "appUserModelId": "App User Model Id value"
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 176

{
  "@odata.type": "#microsoft.graph.microsoftStoreForBusinessContainedApp",
  "id": "bf1d79df-79df-bf1d-df79-1dbfdf791dbf",
  "appUserModelId": "App User Model Id value"
}
```





