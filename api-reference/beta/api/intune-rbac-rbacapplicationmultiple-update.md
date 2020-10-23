---
title: Обновление Рбакаппликатионмултипле
description: Обновление свойств объекта Рбакаппликатионмултипле.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 06fe7e2d7439cb6a92fc8dd21a7d9f37d7b0106e
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48691598"
---
# <a name="update-rbacapplicationmultiple"></a>Обновление Рбакаппликатионмултипле

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Обновление свойств объекта [рбакаппликатионмултипле](../resources/intune-rbac-rbacapplicationmultiple.md) .

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
PATCH /roleManagement/deviceManagement
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Авторизация|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Тело запроса
В тексте запроса добавьте представление объекта [рбакаппликатионмултипле](../resources/intune-rbac-rbacapplicationmultiple.md) в формате JSON.

В следующей таблице приведены свойства, необходимые при создании [рбакаппликатионмултипле](../resources/intune-rbac-rbacapplicationmultiple.md).

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Пока не задокументировано.|



## <a name="response"></a>Ответ
В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [рбакаппликатионмултипле](../resources/intune-rbac-rbacapplicationmultiple.md) в тексте отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
PATCH https://graph.microsoft.com/beta/roleManagement/deviceManagement
Content-type: application/json
Content-length: 65

{
  "@odata.type": "#microsoft.graph.rbacApplicationMultiple"
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 114

{
  "@odata.type": "#microsoft.graph.rbacApplicationMultiple",
  "id": "ee4797e5-97e5-ee47-e597-47eee59747ee"
}
```





