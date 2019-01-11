---
title: checkMemberGroups
description: Проверьте наличие членства в указанный список групп. Возвращает из списка из которых эти группы
author: dkershaw10
localization_priority: Normal
ms.openlocfilehash: 1c9f4da03eee8cf0bc5f1ae15a0886aa42267c7d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27845237"
---
# <a name="checkmembergroups"></a><span data-ttu-id="57032-104">checkMemberGroups</span><span class="sxs-lookup"><span data-stu-id="57032-104">checkMemberGroups</span></span>

> <span data-ttu-id="57032-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="57032-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="57032-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="57032-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="57032-p103">Проверка членства в указанном списке групп. Возвращает из списка те группы, в которых указанный пользователь состоит напрямую или транзитивно.</span><span class="sxs-lookup"><span data-stu-id="57032-p103">Check for membership in the specified list of groups. Returns from the list those groups of which the user has a direct or transitive membership.</span></span>

<span data-ttu-id="57032-p104">В одном запросе можно проверять до 20 групп. Эта функция поддерживает Office 365 и другие типы групп, подготовленных в Azure AD. Обратите внимание, что группы Office 365 не могут содержать групп. Следовательно, членство в группе Office 365 всегда непосредственное.</span><span class="sxs-lookup"><span data-stu-id="57032-p104">You can check up to a maximum of 20 groups per request. This function supports Office 365 and other types of groups provisioned in Azure AD. Note that Office 365 Groups cannot contain groups. So membership in an Office 365 Group is always direct.</span></span>

## <a name="permissions"></a><span data-ttu-id="57032-113">Разрешения</span><span class="sxs-lookup"><span data-stu-id="57032-113">Permissions</span></span>

<span data-ttu-id="57032-p105">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="57032-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="57032-116">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="57032-116">Permission type</span></span>                        | <span data-ttu-id="57032-117">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="57032-117">Permissions (from least to most privileged)</span></span>                                                                        |
| :------------------------------------- | :----------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="57032-118">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="57032-118">Delegated (work or school account)</span></span>     | <span data-ttu-id="57032-119">~~User.Read.All~~, ~~User.ReadWrite.All~~, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="57032-119">~~User.Read.All~~, ~~User.ReadWrite.All~~, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="57032-120">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="57032-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="57032-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="57032-121">Not supported.</span></span>                                                                                                     |
| <span data-ttu-id="57032-122">Для приложения</span><span class="sxs-lookup"><span data-stu-id="57032-122">Application</span></span>                            | <span data-ttu-id="57032-123">~~User.Read.All~~, ~~User.ReadWrite.All~~, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="57032-123">~~User.Read.All~~, ~~User.ReadWrite.All~~, Directory.Read.All, Directory.ReadWrite.All</span></span>                             |

> <span data-ttu-id="57032-124">**Примечание:** Этот интерфейс API в настоящее время требует `Directory.Read.All` разрешений или выше.</span><span class="sxs-lookup"><span data-stu-id="57032-124">**Note:** This API currently requires the `Directory.Read.All` permission or higher.</span></span> <span data-ttu-id="57032-125">С помощью `User.Read.All` или `User.ReadWrite.All` разрешения возвращает ошибку.</span><span class="sxs-lookup"><span data-stu-id="57032-125">Using the `User.Read.All` or `User.ReadWrite.All` permissions will return an error.</span></span> <span data-ttu-id="57032-126">Мы знаем об этой проблеме.</span><span class="sxs-lookup"><span data-stu-id="57032-126">This is a known bug.</span></span>

## <a name="http-request"></a><span data-ttu-id="57032-127">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="57032-127">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /users/{id | userPrincipalName}/checkMemberGroups
```

## <a name="request-headers"></a><span data-ttu-id="57032-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="57032-128">Request headers</span></span>

| <span data-ttu-id="57032-129">Заголовок</span><span class="sxs-lookup"><span data-stu-id="57032-129">Header</span></span>        | <span data-ttu-id="57032-130">Значение</span><span class="sxs-lookup"><span data-stu-id="57032-130">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="57032-131">Авторизация</span><span class="sxs-lookup"><span data-stu-id="57032-131">Authorization</span></span> | <span data-ttu-id="57032-p107">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="57032-p107">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="57032-134">Content-Type</span><span class="sxs-lookup"><span data-stu-id="57032-134">Content-Type</span></span>  | <span data-ttu-id="57032-135">application/json</span><span class="sxs-lookup"><span data-stu-id="57032-135">application/json</span></span>          |

## <a name="request-body"></a><span data-ttu-id="57032-136">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="57032-136">Request body</span></span>

<span data-ttu-id="57032-137">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="57032-137">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="57032-138">Параметр</span><span class="sxs-lookup"><span data-stu-id="57032-138">Parameter</span></span> | <span data-ttu-id="57032-139">Тип</span><span class="sxs-lookup"><span data-stu-id="57032-139">Type</span></span>   | <span data-ttu-id="57032-140">Описание</span><span class="sxs-lookup"><span data-stu-id="57032-140">Description</span></span>           |
| :-------- | :----- | :-------------------- |
| <span data-ttu-id="57032-141">groupIds</span><span class="sxs-lookup"><span data-stu-id="57032-141">groupIds</span></span>  | <span data-ttu-id="57032-142">String</span><span class="sxs-lookup"><span data-stu-id="57032-142">String</span></span> | <span data-ttu-id="57032-143">Массив идентификаторов групп</span><span class="sxs-lookup"><span data-stu-id="57032-143">An array of group ids</span></span> |

## <a name="response"></a><span data-ttu-id="57032-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="57032-144">Response</span></span>

<span data-ttu-id="57032-145">В случае успеха этот метод возвращает код отклика `200 OK` и объект коллекции String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="57032-145">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="57032-146">Пример</span><span class="sxs-lookup"><span data-stu-id="57032-146">Example</span></span>

<span data-ttu-id="57032-147">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="57032-147">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="57032-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="57032-148">Request</span></span>

<span data-ttu-id="57032-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="57032-149">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "user_checkmembergroups"
}-->

```http
POST https://graph.microsoft.com/beta/me/checkMemberGroups
Content-type: application/json
Content-length: 44

{
  "groupIds": [
    "groupIds-value"
  ]
}
```

##### <a name="response"></a><span data-ttu-id="57032-150">Ответ</span><span class="sxs-lookup"><span data-stu-id="57032-150">Response</span></span>

<span data-ttu-id="57032-p108">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="57032-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "string",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 39

{
  "value": [
    "string-value"
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->

<!-- {
  "type": "#page.annotation",
  "description": "user: checkMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
