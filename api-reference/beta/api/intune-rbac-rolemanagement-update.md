---
title: Обновление roleManagement
description: Обновление свойств объекта roleManagement.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2f040cdfbb7a4ddb8e9e84df3917e200e7495cc3
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58796672"
---
# <a name="update-rolemanagement"></a>Обновление roleManagement

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Обновление свойств объекта [roleManagement.](../resources/intune-rbac-rolemanagement.md)

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementRBAC.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Приложение|DeviceManagementRBAC.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /roleManagement
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Authorization|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В теле запроса поставляем представление JSON для [объекта roleManagement.](../resources/intune-rbac-rolemanagement.md)

В следующей таблице показаны свойства, необходимые при создании [roleManagement.](../resources/intune-rbac-rolemanagement.md)

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Пока не задокументировано.|



## <a name="response"></a>Ответ
В случае успешного выполнения этот метод возвращает код ответа и обновленный объект `200 OK` [roleManagement](../resources/intune-rbac-rolemanagement.md) в тексте отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
PATCH https://graph.microsoft.com/beta/roleManagement
Content-type: application/json
Content-length: 56

{
  "@odata.type": "#microsoft.graph.roleManagement"
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 105

{
  "@odata.type": "#microsoft.graph.roleManagement",
  "id": "6fb74c1e-4c1e-6fb7-1e4c-b76f1e4cb76f"
}
```



