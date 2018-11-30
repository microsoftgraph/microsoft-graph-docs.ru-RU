---
title: 'group: checkMemberGroups'
description: Проверьте наличие членства в указанный список групп. Возвращает из списка из которых эти группы
ms.openlocfilehash: d591c4383971155a835d5d6456cdcd3a63803c92
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27078192"
---
# <a name="group-checkmembergroups"></a><span data-ttu-id="9e846-104">group: checkMemberGroups</span><span class="sxs-lookup"><span data-stu-id="9e846-104">group: checkMemberGroups</span></span>

> <span data-ttu-id="9e846-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="9e846-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9e846-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9e846-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9e846-p103">Проверка членства в указанном списке групп. Возвращает из списка те группы, в которых указанная группа состоит напрямую или транзитивно.</span><span class="sxs-lookup"><span data-stu-id="9e846-p103">Check for membership in the specified list of groups. Returns from the list those groups of which the specified group has a direct or transitive membership.</span></span>

<span data-ttu-id="9e846-p104">В одном запросе можно проверять до 20 групп. Эта функция поддерживает Office 365 и другие типы групп, подготовленных в Azure AD. Обратите внимание, что группы Office 365 не могут содержать групп. Следовательно, членство в группе Office 365 всегда непосредственное.</span><span class="sxs-lookup"><span data-stu-id="9e846-p104">You can check up to a maximum of 20 groups per request. This function supports Office 365 and other types of groups provisioned in Azure AD. Note that Office 365 Groups cannot contain groups. So membership in an Office 365 Group is always direct.</span></span>

## <a name="permissions"></a><span data-ttu-id="9e846-113">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9e846-113">Permissions</span></span>

<span data-ttu-id="9e846-p105">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9e846-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9e846-116">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9e846-116">Permission type</span></span>                        | <span data-ttu-id="9e846-117">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9e846-117">Permissions (from least to most privileged)</span></span>                                                 |
| :------------------------------------- | :------------------------------------------------------------------------------------------ |
| <span data-ttu-id="9e846-118">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9e846-118">Delegated (work or school account)</span></span>     | <span data-ttu-id="9e846-119">~~Group.Read.All~~, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="9e846-119">~~Group.Read.All~~, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="9e846-120">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9e846-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9e846-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9e846-121">Not supported.</span></span>                                                                              |
| <span data-ttu-id="9e846-122">Для приложения</span><span class="sxs-lookup"><span data-stu-id="9e846-122">Application</span></span>                            | <span data-ttu-id="9e846-123">~~Group.Read.All~~, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9e846-123">~~Group.Read.All~~, Directory.Read.All, Directory.ReadWrite.All</span></span>                             |

> <span data-ttu-id="9e846-124">**Примечание:** Этот интерфейс API в настоящее время требует `Directory.Read.All` разрешений или выше.</span><span class="sxs-lookup"><span data-stu-id="9e846-124">**Note:** This API currently requires the `Directory.Read.All` permission or higher.</span></span> <span data-ttu-id="9e846-125">С помощью `Group.Read.All` разрешение возвращает ошибку.</span><span class="sxs-lookup"><span data-stu-id="9e846-125">Using the `Group.Read.All` permission will return an error.</span></span> <span data-ttu-id="9e846-126">Мы знаем об этой проблеме.</span><span class="sxs-lookup"><span data-stu-id="9e846-126">This is a known bug.</span></span>

## <a name="http-request"></a><span data-ttu-id="9e846-127">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9e846-127">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /groups/{id}/checkMemberGroups
```

## <a name="request-headers"></a><span data-ttu-id="9e846-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9e846-128">Request headers</span></span>

| <span data-ttu-id="9e846-129">Имя</span><span class="sxs-lookup"><span data-stu-id="9e846-129">Name</span></span>          | <span data-ttu-id="9e846-130">Тип</span><span class="sxs-lookup"><span data-stu-id="9e846-130">Type</span></span>   | <span data-ttu-id="9e846-131">Описание</span><span class="sxs-lookup"><span data-stu-id="9e846-131">Description</span></span>               |
| :------------ | :----- | :------------------------ |
| <span data-ttu-id="9e846-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="9e846-132">Authorization</span></span> | <span data-ttu-id="9e846-133">string</span><span class="sxs-lookup"><span data-stu-id="9e846-133">string</span></span> | <span data-ttu-id="9e846-p107">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9e846-p107">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9e846-136">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9e846-136">Request body</span></span>

<span data-ttu-id="9e846-137">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="9e846-137">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="9e846-138">Параметр</span><span class="sxs-lookup"><span data-stu-id="9e846-138">Parameter</span></span> | <span data-ttu-id="9e846-139">Тип</span><span class="sxs-lookup"><span data-stu-id="9e846-139">Type</span></span>   | <span data-ttu-id="9e846-140">Описание</span><span class="sxs-lookup"><span data-stu-id="9e846-140">Description</span></span>           |
| :-------- | :----- | :-------------------- |
| <span data-ttu-id="9e846-141">groupIds</span><span class="sxs-lookup"><span data-stu-id="9e846-141">groupIds</span></span>  | <span data-ttu-id="9e846-142">String</span><span class="sxs-lookup"><span data-stu-id="9e846-142">String</span></span> | <span data-ttu-id="9e846-143">Массив идентификаторов групп</span><span class="sxs-lookup"><span data-stu-id="9e846-143">An array of group ids</span></span> |

## <a name="response"></a><span data-ttu-id="9e846-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="9e846-144">Response</span></span>

<span data-ttu-id="9e846-145">В случае успеха этот метод возвращает код отклика `200 OK` и объект коллекции String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9e846-145">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9e846-146">Пример</span><span class="sxs-lookup"><span data-stu-id="9e846-146">Example</span></span>

<span data-ttu-id="9e846-147">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="9e846-147">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="9e846-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="9e846-148">Request</span></span>

<span data-ttu-id="9e846-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9e846-149">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "group_checkmembergroups"
}-->

```http
POST https://graph.microsoft.com/beta/groups/{id}/checkMemberGroups
Content-type: application/json
Content-length: 44

{
  "groupIds": [
    "groupIds-value"
  ]
}
```

##### <a name="response"></a><span data-ttu-id="9e846-150">Ответ</span><span class="sxs-lookup"><span data-stu-id="9e846-150">Response</span></span>

<span data-ttu-id="9e846-p108">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="9e846-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
  "description": "group: checkMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
