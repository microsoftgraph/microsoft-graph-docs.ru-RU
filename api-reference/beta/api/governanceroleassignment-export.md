---
title: Экспорт governanceRoleAssignmentRequests
description: Получить коллекцию governanceRoleAssignmentRequests в формате `application/octet-stream`, который можно преобразовать в файл CSV в браузере.
ms.openlocfilehash: 8b9e64faeb8134f5b0bb964d296b1bab309021d9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27076648"
---
# <a name="export-governanceroleassignmentrequests"></a>Экспорт governanceRoleAssignmentRequests

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Получить коллекцию [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) в формате `application/octet-stream`, который можно преобразовать в файл CSV в браузере.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Permissions              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | PrivilegedAccess.ReadWrite.AzureResources  |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|Для приложения | PrivilegedAccess.ReadWrite.AzureResources |


## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->Экспорт коллекции [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) на ресурс
    
>**Примечание:** Помимо области разрешений для этого запроса требуется инициатор запроса может иметь по крайней мере одна роль назначения для ресурса. 
    
```http
GET /privilegedAccess/azureResources/roleAssignments/export?$filter=resourceId+eq+'{resourceId}'
```

Экспорт коллекции [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) Мой
```http
GET /privilegedAccess/azureResources/roleAssignments/export?$filter=subjectId+eq+'{myId}'
```
## <a name="optional-query-parameters"></a>Необязательные параметры запросов
Этот метод поддерживает [Параметры запроса OData](/graph/query-parameters) , которые помогут при настройке клиентов ответа.

## <a name="request-headers"></a>Заголовки запросов
| Имя      |Описание|
|:----------|:----------|
| Authorization  | Bearer {code}|

## <a name="request-body"></a>Текст запроса
Не указывайте тело запроса для этого метода.

## <a name="response"></a>Ответ
Успешно завершена, этот метод возвращает `200 OK` код ответа и содержимое типа `application/octet-stream`.

## <a name="example"></a>Пример
В этом примере сохраняет все назначения ролей в виде CSV-файла в подписке Wingtip Toys - производственного. 

##### <a name="request"></a>Запрос
```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignments/export?filter=resourceId+eq+'85dfe48a-55d3-49fc-8f36-ee14b7f6f720'
```
##### <a name="response"></a>Ответ
Ниже приведен пример отклика. 
```http
HTTP/1.1 200 OK
Content-Type:application/octet-stream
Content-Length:126

77u/77u/QXNzaWdubWVudCBMZXZlbCxVc2VyIEdyb3VwIE5hbWUsUm9sZSBOYW1lLEVtYWlsLEFzc2lnbm1lbnQgVHlwZSxBc3NpZ25tZW43IFN0YXJ0IFRpbWUgKFVUQyksQXNzaWdubWVudCBFbmQgVGltZdAoVVRDKQ0K

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Export governanceRoleAssignmentRequests",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
