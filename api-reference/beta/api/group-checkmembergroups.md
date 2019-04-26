---
title: 'group: checkMemberGroups'
description: Проверка членства в указанном списке групп. Возвращает из списка те группы, в которых
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 1815f187a25eaddbd3b1757fde5e7e4e9c74f650
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33329662"
---
# <a name="group-checkmembergroups"></a><span data-ttu-id="1327d-104">group: checkMemberGroups</span><span class="sxs-lookup"><span data-stu-id="1327d-104">group: checkMemberGroups</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1327d-p102">Проверка членства в указанном списке групп. Возвращает из списка те группы, в которых указанная группа состоит напрямую или транзитивно.</span><span class="sxs-lookup"><span data-stu-id="1327d-p102">Check for membership in the specified list of groups. Returns from the list those groups of which the specified group has a direct or transitive membership.</span></span>

<span data-ttu-id="1327d-p103">В одном запросе можно проверять до 20 групп. Эта функция поддерживает Office 365 и другие типы групп, подготовленных в Azure AD. Обратите внимание, что группы Office 365 не могут содержать групп. Следовательно, членство в группе Office 365 всегда непосредственное.</span><span class="sxs-lookup"><span data-stu-id="1327d-p103">You can check up to a maximum of 20 groups per request. This function supports Office 365 and other types of groups provisioned in Azure AD. Note that Office 365 Groups cannot contain groups. So membership in an Office 365 Group is always direct.</span></span>

## <a name="permissions"></a><span data-ttu-id="1327d-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1327d-111">Permissions</span></span>

<span data-ttu-id="1327d-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1327d-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1327d-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1327d-114">Permission type</span></span>                        | <span data-ttu-id="1327d-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1327d-115">Permissions (from least to most privileged)</span></span>                                                 |
| :------------------------------------- | :------------------------------------------------------------------------------------------ |
| <span data-ttu-id="1327d-116">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1327d-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="1327d-117">~~Group.Read.All~~, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="1327d-117">~~Group.Read.All~~, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="1327d-118">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1327d-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1327d-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1327d-119">Not supported.</span></span>                                                                              |
| <span data-ttu-id="1327d-120">Приложение</span><span class="sxs-lookup"><span data-stu-id="1327d-120">Application</span></span>                            | <span data-ttu-id="1327d-121">~~Group.Read.All~~, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1327d-121">~~Group.Read.All~~, Directory.Read.All, Directory.ReadWrite.All</span></span>                             |

> <span data-ttu-id="1327d-122">**Примечание.** В настоящее время для вызова этого API требуется разрешение `Directory.Read.All` или выше.</span><span class="sxs-lookup"><span data-stu-id="1327d-122">**Note:** This API currently requires the `Directory.Read.All` permission or higher.</span></span> <span data-ttu-id="1327d-123">При использовании разрешения `Group.Read.All` возникает ошибка.</span><span class="sxs-lookup"><span data-stu-id="1327d-123">Using the `Group.Read.All` permission will return an error.</span></span> <span data-ttu-id="1327d-124">Мы знаем об этой проблеме.</span><span class="sxs-lookup"><span data-stu-id="1327d-124">This is a known bug.</span></span>

## <a name="http-request"></a><span data-ttu-id="1327d-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1327d-125">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /groups/{id}/checkMemberGroups
```

## <a name="request-headers"></a><span data-ttu-id="1327d-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1327d-126">Request headers</span></span>

| <span data-ttu-id="1327d-127">Имя</span><span class="sxs-lookup"><span data-stu-id="1327d-127">Name</span></span>          | <span data-ttu-id="1327d-128">Тип</span><span class="sxs-lookup"><span data-stu-id="1327d-128">Type</span></span>   | <span data-ttu-id="1327d-129">Описание</span><span class="sxs-lookup"><span data-stu-id="1327d-129">Description</span></span>               |
| :------------ | :----- | :------------------------ |
| <span data-ttu-id="1327d-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="1327d-130">Authorization</span></span> | <span data-ttu-id="1327d-131">string</span><span class="sxs-lookup"><span data-stu-id="1327d-131">string</span></span> | <span data-ttu-id="1327d-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1327d-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1327d-134">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1327d-134">Request body</span></span>

<span data-ttu-id="1327d-135">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="1327d-135">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="1327d-136">Параметр</span><span class="sxs-lookup"><span data-stu-id="1327d-136">Parameter</span></span> | <span data-ttu-id="1327d-137">Тип</span><span class="sxs-lookup"><span data-stu-id="1327d-137">Type</span></span>   | <span data-ttu-id="1327d-138">Описание</span><span class="sxs-lookup"><span data-stu-id="1327d-138">Description</span></span>           |
| :-------- | :----- | :-------------------- |
| <span data-ttu-id="1327d-139">groupIds</span><span class="sxs-lookup"><span data-stu-id="1327d-139">groupIds</span></span>  | <span data-ttu-id="1327d-140">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="1327d-140">String collection</span></span> | <span data-ttu-id="1327d-141">Массив идентификаторов групп</span><span class="sxs-lookup"><span data-stu-id="1327d-141">An array of group ids</span></span> |

## <a name="response"></a><span data-ttu-id="1327d-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="1327d-142">Response</span></span>

<span data-ttu-id="1327d-143">В случае успеха этот метод возвращает код отклика `200 OK` и объект коллекции String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1327d-143">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1327d-144">Пример</span><span class="sxs-lookup"><span data-stu-id="1327d-144">Example</span></span>

<span data-ttu-id="1327d-145">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="1327d-145">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="1327d-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="1327d-146">Request</span></span>

<span data-ttu-id="1327d-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1327d-147">Here is an example of the request.</span></span>

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

##### <a name="response"></a><span data-ttu-id="1327d-148">Ответ</span><span class="sxs-lookup"><span data-stu-id="1327d-148">Response</span></span>

<span data-ttu-id="1327d-p107">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1327d-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
  "description": "group: checkMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
