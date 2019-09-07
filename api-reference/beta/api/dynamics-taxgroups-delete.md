---
title: Удаление Таксграупс
description: Удаляет объект налоговой группы в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 6374936502929a3a7be3c6822d9145eb0034957c
ms.sourcegitcommit: c68a83d28fa4bfca6e0618467934813a9ae17b12
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/07/2019
ms.locfileid: "36791248"
---
# <a name="delete-taxgroups"></a>Удаление Таксграупс
Удаление объекта налоговой группы из Dynamics 365 Business Central.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения |Разрешения (в порядке повышения привилегий)|
|:---------------|:------------------------------------------|
|Делегированные (рабочая или учебная учетная запись)|Financials.ReadWrite.All |
|Делегированная учетная запись (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|Financials.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос
```
DELETE /financials/companies/{id}/taxGroups/{id}
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов
Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.

## <a name="request-headers"></a>Заголовки запросов
|Заголовок|Значение|
|------|-----|
|Авторизация  |Bearer {токен}. Обязательный. |
|If-Match       |Обязательно. Если этот заголовок запроса включен, а предоставленный тег eTag не отвечает текущему тегу в **таксграупс**, **таксграупс** не будет обновлен. |

## <a name="request-body"></a>Тело запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Ответ
В случае успешного выполнения этот метод возвращает код отклика ```204,No Content```. В тексте отклика не возвращается никаких данных.

## <a name="example"></a>Пример

**Запрос**

Ниже приведен пример запроса.

```json
DELETE https://graph.microsoft.com/beta/financials/companies/{id}/taxGroups/{id}
```

**Отклик** 

Ниже приведен пример отклика. 

```json
HTTP/1.1 204 No Content
```
