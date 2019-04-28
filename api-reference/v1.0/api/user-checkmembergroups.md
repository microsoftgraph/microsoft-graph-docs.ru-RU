---
title: checkMemberGroups
description: Проверка участия в указанном списке групп. Возвращает из списка те группы, в которых
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: a259416525cbd339f68962674a3441c10f6b3235
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32567895"
---
# <a name="checkmembergroups"></a><span data-ttu-id="8f5bc-104">checkMemberGroups</span><span class="sxs-lookup"><span data-stu-id="8f5bc-104">checkMemberGroups</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8f5bc-p102">Проверка участия в указанном списке групп. Возвращает из списка те группы, в которых указанный пользователь состоит напрямую или транзитивно.</span><span class="sxs-lookup"><span data-stu-id="8f5bc-p102">Check for membership in the specified list of groups. Returns from the list those groups of which the user has a direct or transitive membership.</span></span>

<span data-ttu-id="8f5bc-p103">В одном запросе можно проверять до 20 групп. Эта функция поддерживает Office 365 и другие типы групп, подготовленных в Azure AD. Обратите внимание, что группы Office 365 не могут содержать групп. Следовательно, участие в группе Office 365 всегда непосредственное.</span><span class="sxs-lookup"><span data-stu-id="8f5bc-p103">You can check up to a maximum of 20 groups per request. This function supports Office 365 and other types of groups provisioned in Azure AD. Note that Office 365 Groups cannot contain groups. So membership in an Office 365 Group is always direct.</span></span>

## <a name="permissions"></a><span data-ttu-id="8f5bc-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8f5bc-111">Permissions</span></span>

<span data-ttu-id="8f5bc-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8f5bc-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8f5bc-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8f5bc-114">Permission type</span></span>                        | <span data-ttu-id="8f5bc-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8f5bc-115">Permissions (from least to most privileged)</span></span>                                                                        |
| :------------------------------------- | :----------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="8f5bc-116">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8f5bc-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="8f5bc-117">~~User.Read.All~~, ~~User.ReadWrite.All~~, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="8f5bc-117">~~User.Read.All~~, ~~User.ReadWrite.All~~, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="8f5bc-118">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8f5bc-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8f5bc-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8f5bc-119">Not supported.</span></span>                                                                                                     |
| <span data-ttu-id="8f5bc-120">Для приложения</span><span class="sxs-lookup"><span data-stu-id="8f5bc-120">Application</span></span>                            | <span data-ttu-id="8f5bc-121">~~User.Read.All~~, ~~User.ReadWrite.All~~, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8f5bc-121">~~User.Read.All~~, ~~User.ReadWrite.All~~, Directory.Read.All, Directory.ReadWrite.All</span></span>                             |

> <span data-ttu-id="8f5bc-122">**Примечание.** В настоящее время для вызова этого API требуется разрешение `Directory.Read.All` или выше.</span><span class="sxs-lookup"><span data-stu-id="8f5bc-122">Note: This API currently requires the Directory.Read.All permission or higher.</span></span> <span data-ttu-id="8f5bc-123">При использовании разрешений `User.Read.All` или `User.ReadWrite.All` возникает ошибка.</span><span class="sxs-lookup"><span data-stu-id="8f5bc-123">Using the User.Read.All or User.ReadWrite.All permissions will return an error.</span></span> <span data-ttu-id="8f5bc-124">Мы знаем об этой проблеме.</span><span class="sxs-lookup"><span data-stu-id="8f5bc-124">This is a known bug.</span></span>

## <a name="http-request"></a><span data-ttu-id="8f5bc-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8f5bc-125">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /users/{id | userPrincipalName}/checkMemberGroups
```

## <a name="request-headers"></a><span data-ttu-id="8f5bc-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8f5bc-126">Request headers</span></span>

| <span data-ttu-id="8f5bc-127">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8f5bc-127">Header</span></span>        | <span data-ttu-id="8f5bc-128">Значение</span><span class="sxs-lookup"><span data-stu-id="8f5bc-128">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="8f5bc-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8f5bc-129">Authorization</span></span> | <span data-ttu-id="8f5bc-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8f5bc-p106">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8f5bc-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8f5bc-132">Content-Type</span></span>  | <span data-ttu-id="8f5bc-133">application/json</span><span class="sxs-lookup"><span data-stu-id="8f5bc-133">application/json</span></span>          |

## <a name="request-body"></a><span data-ttu-id="8f5bc-134">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8f5bc-134">Request body</span></span>

<span data-ttu-id="8f5bc-135">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="8f5bc-135">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="8f5bc-136">Параметр</span><span class="sxs-lookup"><span data-stu-id="8f5bc-136">Parameter</span></span> | <span data-ttu-id="8f5bc-137">Тип</span><span class="sxs-lookup"><span data-stu-id="8f5bc-137">Type</span></span>   | <span data-ttu-id="8f5bc-138">Описание</span><span class="sxs-lookup"><span data-stu-id="8f5bc-138">Description</span></span>           |
| :-------- | :----- | :-------------------- |
| <span data-ttu-id="8f5bc-139">groupIds</span><span class="sxs-lookup"><span data-stu-id="8f5bc-139">groupIds</span></span>  | <span data-ttu-id="8f5bc-140">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="8f5bc-140">String collection</span></span> | <span data-ttu-id="8f5bc-141">Массив идентификаторов групп</span><span class="sxs-lookup"><span data-stu-id="8f5bc-141">An array of group ids</span></span> |

## <a name="response"></a><span data-ttu-id="8f5bc-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="8f5bc-142">Response</span></span>

<span data-ttu-id="8f5bc-143">В случае успеха этот метод возвращает код отклика `200 OK` и объект коллекции String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8f5bc-143">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8f5bc-144">Пример</span><span class="sxs-lookup"><span data-stu-id="8f5bc-144">Example</span></span>

<span data-ttu-id="8f5bc-145">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="8f5bc-145">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="8f5bc-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="8f5bc-146">Request</span></span>

<span data-ttu-id="8f5bc-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8f5bc-147">Here is an example of the request.</span></span>

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

##### <a name="response"></a><span data-ttu-id="8f5bc-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="8f5bc-148">Response</span></span>

<span data-ttu-id="8f5bc-p107">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8f5bc-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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

<!--
{
  "type": "#page.annotation",
  "description": "user: checkMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
