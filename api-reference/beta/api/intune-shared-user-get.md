---
title: Получение пользователя
description: Чтение свойств и связей объекта user.
author: rolyon
ms.localizationpriority: medium
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: bb961869dcd754a0f9a6baa987362622b580b9c9
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59064660"
---
# <a name="get-user"></a>Получение пользователя

Пространство имен: microsoft.graph

> **Важно:** API в версии /бета-версии в Microsoft Graph могут изменяться. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Чтение свойств и связей объекта [user](../resources/intune-shared-user.md).

## <a name="prerequisites"></a>Необходимые компоненты

Для вызова этого API требуется одно из следующих разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).  Конкретное разрешение зависит от контекста.

|Тип разрешения|Разрешения (в порядке убывания привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)||
| &nbsp; &nbsp; **Управление устройствами** | DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All |
| &nbsp;&nbsp; **MAM** | DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All |
| &nbsp; &nbsp; **Адаптация** | DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All |
| &nbsp; &nbsp; **Устранение неполадок** | DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All |
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений||
| &nbsp; &nbsp; **Управление устройствами** | DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All |
| &nbsp;&nbsp; **MAM** | DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All |
| &nbsp; &nbsp; **Адаптация** | DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All |
| &nbsp; &nbsp; **Устранение неполадок** | DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All |

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов

Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.

## <a name="request-headers"></a>Заголовки запросов

|Заголовок|Значение|
|:---|:---|
|Authorization|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса

Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успеха этот метод возвращает код отклика `200 OK` и объект [user](../resources/intune-shared-user.md) в тексте отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос

Ниже приведен пример запроса.

``` http
GET https://graph.microsoft.com/beta/users/{usersId}
```

### <a name="response"></a>Отклик

Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 118

{
  "value": {
    "@odata.type": "#microsoft.graph.user",
    "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3"
  }
}
```









