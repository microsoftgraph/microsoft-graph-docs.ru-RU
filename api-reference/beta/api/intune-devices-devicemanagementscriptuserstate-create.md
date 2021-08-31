---
title: Создание deviceManagementScriptUserState
description: Создайте новый объект deviceManagementScriptUserState.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 564f4b94168f193ab8d6dbb27c0fd98a25d5edbc
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58783724"
---
# <a name="create-devicemanagementscriptuserstate"></a>Создание deviceManagementScriptUserState

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Создайте новый [объект deviceManagementScriptUserState.](../resources/intune-devices-devicemanagementscriptuserstate.md)

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementManagedDevices.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Application|DeviceManagementManagedDevices.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceShellScripts/{deviceShellScriptId}/userRunStates
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/userRunStates
POST /deviceManagement/deviceCustomAttributeShellScripts/{deviceCustomAttributeShellScriptId}/userRunStates
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Authorization|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В теле запроса укажи представление JSON для объекта deviceManagementScriptUserState.

В следующей таблице показаны свойства, необходимые при создании устройстваManagementScriptUserState.

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Ключ пользовательского состояния скрипта управления устройствами. Это свойство доступно только для чтения.|
|successDeviceCount|Int32|Количество устройств успешности для определенного пользователя.|
|errorDeviceCount|Int32|Количество устройств ошибки для определенного пользователя.|
|userPrincipalName|String|Имя принципа пользователя конкретного пользователя.|



## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает код отклика и `201 Created` [объект deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md) в тексте ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceShellScripts/{deviceShellScriptId}/userRunStates
Content-type: application/json
Content-length: 180

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptUserState",
  "successDeviceCount": 2,
  "errorDeviceCount": 0,
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 229

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptUserState",
  "id": "d5a29103-9103-d5a2-0391-a2d50391a2d5",
  "successDeviceCount": 2,
  "errorDeviceCount": 0,
  "userPrincipalName": "User Principal Name value"
}
```



