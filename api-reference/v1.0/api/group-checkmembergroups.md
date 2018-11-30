---
title: 'group: checkMemberGroups'
description: Проверьте наличие членства в указанный список групп. Возвращает из списка из которых эти группы
ms.openlocfilehash: d0dc617300e29950e820dd94701173829fa6bb7b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27026354"
---
# <a name="group-checkmembergroups"></a><span data-ttu-id="e5457-104">group: checkMemberGroups</span><span class="sxs-lookup"><span data-stu-id="e5457-104">group: checkMemberGroups</span></span>

<span data-ttu-id="e5457-p102">Проверка членства в указанном списке групп. Возвращает из списка те группы, в которых указанная группа состоит напрямую или транзитивно.</span><span class="sxs-lookup"><span data-stu-id="e5457-p102">Check for membership in the specified list of groups. Returns from the list those groups of which the specified group has a direct or transitive membership.</span></span>

<span data-ttu-id="e5457-p103">В одном запросе можно проверять до 20 групп. Эта функция поддерживает Office 365 и другие типы групп, подготовленных в Azure AD. Обратите внимание, что группы Office 365 не могут содержать групп. Следовательно, членство в группе Office 365 всегда непосредственное.</span><span class="sxs-lookup"><span data-stu-id="e5457-p103">You can check up to a maximum of 20 groups per request. This function supports Office 365 and other types of groups provisioned in Azure AD. Note that Office 365 Groups cannot contain groups. So membership in an Office 365 Group is always direct.</span></span>

## <a name="permissions"></a><span data-ttu-id="e5457-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e5457-111">Permissions</span></span>

<span data-ttu-id="e5457-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e5457-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e5457-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e5457-114">Permission type</span></span>                        | <span data-ttu-id="e5457-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e5457-115">Permissions (from least to most privileged)</span></span>                                                 |
| :------------------------------------- | :------------------------------------------------------------------------------------------ |
| <span data-ttu-id="e5457-116">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e5457-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="e5457-117">~~Group.Read.All~~, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e5457-117">~~Group.Read.All~~, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="e5457-118">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e5457-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e5457-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e5457-119">Not supported.</span></span>                                                                              |
| <span data-ttu-id="e5457-120">Для приложения</span><span class="sxs-lookup"><span data-stu-id="e5457-120">Application</span></span>                            | <span data-ttu-id="e5457-121">_Group.Read.All_, Directory.Read.All.</span><span class="sxs-lookup"><span data-stu-id="e5457-121">_Group.Read.All_, Directory.Read.All.</span></span> <span data-ttu-id="e5457-122">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e5457-122">Directory.ReadWrite.All</span></span>                               |

> <span data-ttu-id="e5457-123">**Примечание:** Этот интерфейс API в настоящее время требует `Directory.Read.All` разрешений или выше.</span><span class="sxs-lookup"><span data-stu-id="e5457-123">**Note:** This API currently requires the `Directory.Read.All` permission or higher.</span></span> <span data-ttu-id="e5457-124">С помощью `Group.Read.All` разрешение возвращает ошибку.</span><span class="sxs-lookup"><span data-stu-id="e5457-124">Using the `Group.Read.All` permission will return an error.</span></span> <span data-ttu-id="e5457-125">Мы знаем об этой проблеме.</span><span class="sxs-lookup"><span data-stu-id="e5457-125">This is a known bug.</span></span>

## <a name="http-request"></a><span data-ttu-id="e5457-126">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e5457-126">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /groups/{id}/checkMemberGroups
```

## <a name="request-headers"></a><span data-ttu-id="e5457-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e5457-127">Request headers</span></span>

| <span data-ttu-id="e5457-128">Имя</span><span class="sxs-lookup"><span data-stu-id="e5457-128">Name</span></span>          | <span data-ttu-id="e5457-129">Тип</span><span class="sxs-lookup"><span data-stu-id="e5457-129">Type</span></span>   | <span data-ttu-id="e5457-130">Описание</span><span class="sxs-lookup"><span data-stu-id="e5457-130">Description</span></span>               |
| :------------ | :----- | :------------------------ |
| <span data-ttu-id="e5457-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="e5457-131">Authorization</span></span> | <span data-ttu-id="e5457-132">string</span><span class="sxs-lookup"><span data-stu-id="e5457-132">string</span></span> | <span data-ttu-id="e5457-p107">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e5457-p107">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e5457-135">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e5457-135">Request body</span></span>

<span data-ttu-id="e5457-136">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="e5457-136">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="e5457-137">Параметр</span><span class="sxs-lookup"><span data-stu-id="e5457-137">Parameter</span></span> | <span data-ttu-id="e5457-138">Тип</span><span class="sxs-lookup"><span data-stu-id="e5457-138">Type</span></span>              | <span data-ttu-id="e5457-139">Описание</span><span class="sxs-lookup"><span data-stu-id="e5457-139">Description</span></span>           |
| :-------- | :---------------- | :-------------------- |
| <span data-ttu-id="e5457-140">groupIds</span><span class="sxs-lookup"><span data-stu-id="e5457-140">groupIds</span></span>  | <span data-ttu-id="e5457-141">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="e5457-141">String collection</span></span> | <span data-ttu-id="e5457-142">Массив идентификаторов групп</span><span class="sxs-lookup"><span data-stu-id="e5457-142">An array of group ids</span></span> |

## <a name="response"></a><span data-ttu-id="e5457-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="e5457-143">Response</span></span>

<span data-ttu-id="e5457-144">В случае успеха этот метод возвращает код отклика `200 OK` и объект коллекции String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e5457-144">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e5457-145">Пример</span><span class="sxs-lookup"><span data-stu-id="e5457-145">Example</span></span>

<span data-ttu-id="e5457-146">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="e5457-146">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="e5457-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="e5457-147">Request</span></span>

<span data-ttu-id="e5457-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e5457-148">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "group_checkmembergroups"
}-->

```http
POST https://graph.microsoft.com/v1.0/groups/{id}/checkMemberGroups
Content-type: application/json
Content-length: 44

{
  "groupIds": [
    "groupIds-value"
  ]
}
```

##### <a name="response"></a><span data-ttu-id="e5457-149">Ответ</span><span class="sxs-lookup"><span data-stu-id="e5457-149">Response</span></span>

<span data-ttu-id="e5457-p108">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="e5457-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
