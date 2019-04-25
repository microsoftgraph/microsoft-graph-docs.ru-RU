---
title: checkMemberGroups
description: Проверка членства в указанном списке групп. Возвращает список этих групп, из которых
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 0d7452795cb0a8ffdf3a966a3e350a8634b2a7ad
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32536806"
---
# <a name="checkmembergroups"></a><span data-ttu-id="17ed3-104">checkMemberGroups</span><span class="sxs-lookup"><span data-stu-id="17ed3-104">checkMemberGroups</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="17ed3-p102">Проверка членства в указанном списке групп. Возвращает из списка те группы, в которых указанный пользователь состоит напрямую или транзитивно.</span><span class="sxs-lookup"><span data-stu-id="17ed3-p102">Check for membership in the specified list of groups. Returns from the list those groups of which the user has a direct or transitive membership.</span></span>

<span data-ttu-id="17ed3-p103">В одном запросе можно проверять до 20 групп. Эта функция поддерживает Office 365 и другие типы групп, подготовленных в Azure AD. Обратите внимание, что группы Office 365 не могут содержать групп. Следовательно, членство в группе Office 365 всегда непосредственное.</span><span class="sxs-lookup"><span data-stu-id="17ed3-p103">You can check up to a maximum of 20 groups per request. This function supports Office 365 and other types of groups provisioned in Azure AD. Note that Office 365 Groups cannot contain groups. So membership in an Office 365 Group is always direct.</span></span>

## <a name="permissions"></a><span data-ttu-id="17ed3-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="17ed3-111">Permissions</span></span>

<span data-ttu-id="17ed3-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="17ed3-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="17ed3-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="17ed3-114">Permission type</span></span>                        | <span data-ttu-id="17ed3-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="17ed3-115">Permissions (from least to most privileged)</span></span>                                                                        |
| :------------------------------------- | :----------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="17ed3-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="17ed3-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="17ed3-117">~~User.Read.All~~, ~~User.ReadWrite.All~~, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="17ed3-117">~~User.Read.All~~, ~~User.ReadWrite.All~~, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="17ed3-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="17ed3-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="17ed3-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="17ed3-119">Not supported.</span></span>                                                                                                     |
| <span data-ttu-id="17ed3-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="17ed3-120">Application</span></span>                            | <span data-ttu-id="17ed3-121">~~User.Read.All~~, ~~User.ReadWrite.All~~, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="17ed3-121">~~User.Read.All~~, ~~User.ReadWrite.All~~, Directory.Read.All, Directory.ReadWrite.All</span></span>                             |

> <span data-ttu-id="17ed3-122">**Примечание:** Этот API на `Directory.Read.All` данный момент требует разрешение или более высокий уровень.</span><span class="sxs-lookup"><span data-stu-id="17ed3-122">**Note:** This API currently requires the `Directory.Read.All` permission or higher.</span></span> <span data-ttu-id="17ed3-123">При использовании `User.Read.All` разрешений `User.ReadWrite.All` или разрешений возвращается ошибка.</span><span class="sxs-lookup"><span data-stu-id="17ed3-123">Using the `User.Read.All` or `User.ReadWrite.All` permissions will return an error.</span></span> <span data-ttu-id="17ed3-124">Мы знаем об этой проблеме.</span><span class="sxs-lookup"><span data-stu-id="17ed3-124">This is a known bug.</span></span>

## <a name="http-request"></a><span data-ttu-id="17ed3-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="17ed3-125">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /users/{id | userPrincipalName}/checkMemberGroups
```

## <a name="request-headers"></a><span data-ttu-id="17ed3-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="17ed3-126">Request headers</span></span>

| <span data-ttu-id="17ed3-127">Заголовок</span><span class="sxs-lookup"><span data-stu-id="17ed3-127">Header</span></span>        | <span data-ttu-id="17ed3-128">Значение</span><span class="sxs-lookup"><span data-stu-id="17ed3-128">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="17ed3-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="17ed3-129">Authorization</span></span> | <span data-ttu-id="17ed3-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="17ed3-p106">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="17ed3-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="17ed3-132">Content-Type</span></span>  | <span data-ttu-id="17ed3-133">application/json</span><span class="sxs-lookup"><span data-stu-id="17ed3-133">application/json</span></span>          |

## <a name="request-body"></a><span data-ttu-id="17ed3-134">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="17ed3-134">Request body</span></span>

<span data-ttu-id="17ed3-135">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="17ed3-135">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="17ed3-136">Параметр</span><span class="sxs-lookup"><span data-stu-id="17ed3-136">Parameter</span></span> | <span data-ttu-id="17ed3-137">Тип</span><span class="sxs-lookup"><span data-stu-id="17ed3-137">Type</span></span>   | <span data-ttu-id="17ed3-138">Описание</span><span class="sxs-lookup"><span data-stu-id="17ed3-138">Description</span></span>           |
| :-------- | :----- | :-------------------- |
| <span data-ttu-id="17ed3-139">groupIds</span><span class="sxs-lookup"><span data-stu-id="17ed3-139">groupIds</span></span>  | <span data-ttu-id="17ed3-140">String</span><span class="sxs-lookup"><span data-stu-id="17ed3-140">String</span></span> | <span data-ttu-id="17ed3-141">Массив идентификаторов групп</span><span class="sxs-lookup"><span data-stu-id="17ed3-141">An array of group ids</span></span> |

## <a name="response"></a><span data-ttu-id="17ed3-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="17ed3-142">Response</span></span>

<span data-ttu-id="17ed3-143">В случае успеха этот метод возвращает код отклика `200 OK` и объект коллекции String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="17ed3-143">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="17ed3-144">Пример</span><span class="sxs-lookup"><span data-stu-id="17ed3-144">Example</span></span>

<span data-ttu-id="17ed3-145">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="17ed3-145">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="17ed3-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="17ed3-146">Request</span></span>

<span data-ttu-id="17ed3-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="17ed3-147">Here is an example of the request.</span></span>

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

##### <a name="response"></a><span data-ttu-id="17ed3-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="17ed3-148">Response</span></span>

<span data-ttu-id="17ed3-p107">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="17ed3-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/api/user-checkmembergroups.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
