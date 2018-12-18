---
title: Создайте параметр каталога на группы
description: Используйте этот интерфейс API для создания нового параметра каталог для группы.
author: dkershaw10
ms.openlocfilehash: 2e400babc809bdc8d9277cad1bd41b8b714e4e92
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27358998"
---
# <a name="create-a-directory-setting-on-groups"></a><span data-ttu-id="b0d2c-103">Создайте параметр каталога на группы</span><span class="sxs-lookup"><span data-stu-id="b0d2c-103">Create a directory setting on groups</span></span>

> <span data-ttu-id="b0d2c-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="b0d2c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b0d2c-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b0d2c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b0d2c-106">Используйте этот интерфейс API для создания нового параметра каталог для группы.</span><span class="sxs-lookup"><span data-stu-id="b0d2c-106">Use this API to create a new directory setting for the group.</span></span>
## <a name="permissions"></a><span data-ttu-id="b0d2c-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b0d2c-107">Permissions</span></span>
<span data-ttu-id="b0d2c-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b0d2c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b0d2c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b0d2c-110">Permission type</span></span>      | <span data-ttu-id="b0d2c-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b0d2c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b0d2c-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b0d2c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="b0d2c-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b0d2c-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="b0d2c-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b0d2c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b0d2c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b0d2c-115">Not supported.</span></span>    |
|<span data-ttu-id="b0d2c-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b0d2c-116">Application</span></span> | <span data-ttu-id="b0d2c-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b0d2c-117">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b0d2c-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b0d2c-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/settings
```
## <a name="request-headers"></a><span data-ttu-id="b0d2c-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b0d2c-119">Request headers</span></span>
| <span data-ttu-id="b0d2c-120">Имя</span><span class="sxs-lookup"><span data-stu-id="b0d2c-120">Name</span></span>       | <span data-ttu-id="b0d2c-121">Описание</span><span class="sxs-lookup"><span data-stu-id="b0d2c-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="b0d2c-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b0d2c-122">Authorization</span></span>  | <span data-ttu-id="b0d2c-123">Носителя <token>.</span><span class="sxs-lookup"><span data-stu-id="b0d2c-123">Bearer <token>.</span></span> <span data-ttu-id="b0d2c-124">Обязательное</span><span class="sxs-lookup"><span data-stu-id="b0d2c-124">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="b0d2c-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b0d2c-125">Request body</span></span>
<span data-ttu-id="b0d2c-126">В тексте запроса укажите представление JSON объекта [directorySetting](../resources/directorysetting.md) .</span><span class="sxs-lookup"><span data-stu-id="b0d2c-126">In the request body, supply a JSON representation of [directorySetting](../resources/directorysetting.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="b0d2c-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="b0d2c-127">Response</span></span>

<span data-ttu-id="b0d2c-128">Успешно завершена, этот метод возвращает `201 Created` объект [directorySetting](../resources/directorysetting.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="b0d2c-128">If successful, this method returns `201 Created` response code and [directorySetting](../resources/directorysetting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b0d2c-129">Пример</span><span class="sxs-lookup"><span data-stu-id="b0d2c-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b0d2c-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="b0d2c-130">Request</span></span>
<span data-ttu-id="b0d2c-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b0d2c-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directorysetting_from_group"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/settings
Content-type: application/json
Content-length: 222

{
  "directorySetting": {
    "displayName": "displayName-value",
    "templateId": "templateId-value",
    "values": [
      {
        "name": "name-value",
        "value": "value-value"
      }
    ]
  }
}
```
<span data-ttu-id="b0d2c-132">В тексте запроса укажите представление JSON объекта [directorySetting](../resources/directorysetting.md) .</span><span class="sxs-lookup"><span data-stu-id="b0d2c-132">In the request body, supply a JSON representation of [directorySetting](../resources/directorysetting.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="b0d2c-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="b0d2c-133">Response</span></span>
<span data-ttu-id="b0d2c-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="b0d2c-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directorySetting"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 244

{
  "directorySetting": {
    "id": "id-value",
    "displayName": "displayName-value",
    "templateId": "templateId-value",
    "values": [
      {
        "name": "name-value",
        "value": "value-value"
      }
    ]
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create directorySetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->