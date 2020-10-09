---
title: Список "Общие"
description: Расчетные данные, возвращающие список файлов, которыми вы поделились с пользователем.
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: apiPageType
ms.openlocfilehash: 5ee215dff7fafaa25e4601ade1819322d8894e5a
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/09/2020
ms.locfileid: "48401577"
---
# <a name="list-shared"></a>Список "Общие"

Пространство имен: microsoft.graph

Вычисляемое представление, включающее список документов, к которым пользователь предоставил доступ.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Sites.Read.All, Sites.ReadWrite.All    |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|Для приложений | Sites.Read.All, Sites.ReadWrite.All |

## <a name="http-request"></a>HTTP-запрос
Получение списка документов, доступ к которым предоставлен вошедшего пользователя.

>**Note**: только пользователь может выполнять запросы, используя идентификатор пользователя или имя субъекта.

```http
GET /me/insights/shared
GET /users/{id | userPrincipalName}/insights/shared
```

Разверните ресурс, на который ссылается **совместное** представление:
```http
GET https://graph.microsoft.com/v1.0/me/insights/shared/{id}/resource
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов
Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.

`$filter`С помощью параметра запроса можно фильтровать общие элементы. Например, на основе **типа**:

`https://graph.microsoft.com/v1.0/me/insights/shared?$filter=ResourceVisualization/Type eq 'PowerPoint'`

Просмотрите доступные типы и типы контейнеров, которые можно фильтровать в [ресурсе resourcevisualization](../resources/insights-resourcevisualization.md).

Вы также можете получить файлы, к которым предоставлен доступ конкретному пользователю. Например, указав `lastshared/sharedby/address` свойство:

`https://graph.microsoft.com/v1.0/me/insights/shared?$filter=lastshared/sharedby/address eq 'kellygraham@contoso.com'`

Просмотр сложного типа [шарингдетаил](../resources/insights-sharingdetail.md) .


## <a name="request-headers"></a>Заголовки запросов
| Заголовок       |  Значение|
|:-------------|:------|
| Авторизация  | Bearer {токен}. Обязательный.|
| Accept  | application/json|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает `200 OK` код отклика и список [общих](../resources/insights-shared.md) элементов в теле отклика.
## <a name="example"></a>Пример

##### <a name="request"></a>Запрос

Ниже приведен пример запроса.
```http
GET https://graph.microsoft.com/v1.0/me/insights/shared
```

##### <a name="response"></a>Отклик

Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
```http
{
    "value": [
        {   
            "id": "id-value",
            "lastShared" : { 
                "sharedDateTime" : "sharedDateTime-value",  
                "sharingSubject" : "sharingSubject-value",
                "sharingType" : "sharingType-value", 
                "sharedBy" : { 
                    "displayName" : "displayName-value", 
                    "id": "id-value" 
                }
                "sharingReference" : { 
                    "webUrl" : "webUrl-value",
                    "type: "type-value", 
                    "id": "id-value"
                } 
            },
            "resourceVisualization": { 
                "title" : "title-value, 
                "type"  : "type-value",
                "mediaType" : "mediaType-value",
                "previewImageUrl" : previewImageUrl-value, 
                "previewText" : "previewText-value", 
                "containerWebUrl" : "containerWebUrl-value", 
                "containerDisplayName" : "containerDisplayName-value", 
                "containerType" : "containerType-value" 
            }, 
            "resourceReference" : { 
                "webUrl" : "webUrl-value", 
                "id": "id-value", 
                "type: "type-value" 
}
```