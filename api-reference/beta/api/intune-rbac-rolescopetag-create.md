---
title: Создание Ролескопетаг
description: Создание нового объекта Ролескопетаг.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b974205746ab7e50ceff1dd10de2238e1d8ab624
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39955163"
---
# <a name="create-rolescopetag"></a>Создание Ролескопетаг

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Создание нового объекта [ролескопетаг](../resources/intune-rbac-rolescopetag.md) .

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке убывания привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementRBAC.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|DeviceManagementRBAC.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleScopeTags
POST /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/microsoft.graph.deviceAndAppManagementRoleAssignment/roleScopeTags
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Авторизация|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Тело запроса
В тексте запроса добавьте представление объекта Ролескопетаг в формате JSON.

В следующей таблице приведены свойства, необходимые при создании Ролескопетаг.

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта. Это свойство доступно только для чтения и создается автоматически.|
|displayName|Строка|Отображаемое или понятное имя тега области применения роли.|
|description|String|Описание тега области применения роли.|
|isBuiltIn|Boolean|Описание тега области применения роли.|



## <a name="response"></a>Ответ
В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [ролескопетаг](../resources/intune-rbac-rolescopetag.md) в тексте отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/roleScopeTags
Content-type: application/json
Content-length: 155

{
  "@odata.type": "#microsoft.graph.roleScopeTag",
  "displayName": "Display Name value",
  "description": "Description value",
  "isBuiltIn": true
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 204

{
  "@odata.type": "#microsoft.graph.roleScopeTag",
  "id": "9ed1e179-e179-9ed1-79e1-d19e79e1d19e",
  "displayName": "Display Name value",
  "description": "Description value",
  "isBuiltIn": true
}
```





