---
title: 'user: getMemberGroups'
description: Возвращает все группы, в которые входит пользователь. Проверка доверия транзитивных, в отличие от чтения
localization_priority: Normal
ms.openlocfilehash: 097d6d6eafa031bf86460e97ced58d0063eee4ed
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27879788"
---
# <a name="user-getmembergroups"></a><span data-ttu-id="93103-104">user: getMemberGroups</span><span class="sxs-lookup"><span data-stu-id="93103-104">user: getMemberGroups</span></span>

> <span data-ttu-id="93103-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="93103-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="93103-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="93103-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="93103-p103">Возвращение всех названий групп, в которых состоит пользователь. Проверка промежуточная, в отличие от считывания свойства навигации [memberOf](../api/user-list-memberof.md) (возвращаются только группы, для которых пользователь является непосредственным членом).</span><span class="sxs-lookup"><span data-stu-id="93103-p103">Return all the groups that the user is a member of. The check is transitive, unlike reading the [memberOf](../api/user-list-memberof.md) navigation property, which returns only the groups that the user is a direct member of.</span></span>

<span data-ttu-id="93103-p104">Эта функция поддерживает Office 365 и другие типы групп, подготовленных к работе в Azure AD. Максимальное количество групп, которые может вернуть каждый запрос, — 2046. Обратите внимание, что компонент "Группы Office 365" не может содержать группы. Следовательно, членство, относящееся к компоненту "Группы Office 365", всегда непосредственное.</span><span class="sxs-lookup"><span data-stu-id="93103-p104">This function supports Office 365 and other types of groups provisioned in Azure AD. The maximum number of groups each request can return is 2046. Note that Office 365 Groups cannot contain groups. So membership in an Office 365 Group is always direct.</span></span>

## <a name="permissions"></a><span data-ttu-id="93103-113">Разрешения</span><span class="sxs-lookup"><span data-stu-id="93103-113">Permissions</span></span>

<span data-ttu-id="93103-p105">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="93103-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="93103-116">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="93103-116">Permission type</span></span>                        | <span data-ttu-id="93103-117">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="93103-117">Permissions (from least to most privileged)</span></span>                                                                                                          |
| :------------------------------------- | :--------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="93103-118">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="93103-118">Delegated (work or school account)</span></span>     | <span data-ttu-id="93103-119">~~User.Read и Group.Read.All~~, ~~User.ReadBasic.All и Group.Read.All~~, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="93103-119">~~User.Read and Group.Read.All~~, ~~User.ReadBasic.All and Group.Read.All~~, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="93103-120">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="93103-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="93103-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="93103-121">Not supported.</span></span>                                                                                                                                       |
| <span data-ttu-id="93103-122">Для приложения</span><span class="sxs-lookup"><span data-stu-id="93103-122">Application</span></span>                            | <span data-ttu-id="93103-123">_Group.Read.All_, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="93103-123">_Group.Read.All_, Directory.Read.All, Directory.ReadWrite.All</span></span>                                                                                        |

> <span data-ttu-id="93103-124">**Примечание:** Этот интерфейс API в настоящее время требует `Directory.Read.All` разрешений или выше.</span><span class="sxs-lookup"><span data-stu-id="93103-124">**Note:** This API currently requires the `Directory.Read.All` permission or higher.</span></span> <span data-ttu-id="93103-125">С помощью разрешений Group.Read.All, отдельно или в сочетании с `User.` разрешений, возвращается ошибка.</span><span class="sxs-lookup"><span data-stu-id="93103-125">Using the Group.Read.All permission, either alone or in combination with a `User.` permission, will return an error.</span></span> <span data-ttu-id="93103-126">Мы знаем об этой проблеме.</span><span class="sxs-lookup"><span data-stu-id="93103-126">This is a known bug.</span></span>

## <a name="http-request"></a><span data-ttu-id="93103-127">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="93103-127">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /users/{id | userPrincipalName}/getMemberGroups
```

## <a name="request-headers"></a><span data-ttu-id="93103-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="93103-128">Request headers</span></span>

| <span data-ttu-id="93103-129">Заголовок</span><span class="sxs-lookup"><span data-stu-id="93103-129">Header</span></span>        | <span data-ttu-id="93103-130">Значение</span><span class="sxs-lookup"><span data-stu-id="93103-130">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="93103-131">Авторизация</span><span class="sxs-lookup"><span data-stu-id="93103-131">Authorization</span></span> | <span data-ttu-id="93103-p107">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="93103-p107">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="93103-134">Content-Type</span><span class="sxs-lookup"><span data-stu-id="93103-134">Content-Type</span></span>  | <span data-ttu-id="93103-135">application/json</span><span class="sxs-lookup"><span data-stu-id="93103-135">application/json</span></span>          |

## <a name="request-body"></a><span data-ttu-id="93103-136">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="93103-136">Request body</span></span>

<span data-ttu-id="93103-137">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="93103-137">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="93103-138">Параметр</span><span class="sxs-lookup"><span data-stu-id="93103-138">Parameter</span></span>           | <span data-ttu-id="93103-139">Тип</span><span class="sxs-lookup"><span data-stu-id="93103-139">Type</span></span>    | <span data-ttu-id="93103-140">Описание</span><span class="sxs-lookup"><span data-stu-id="93103-140">Description</span></span>                                                                                                                                                                                                                                                                         |
| :------------------ | :------ | :---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="93103-141">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="93103-141">securityEnabledOnly</span></span> | <span data-ttu-id="93103-142">Логическое</span><span class="sxs-lookup"><span data-stu-id="93103-142">Boolean</span></span> | <span data-ttu-id="93103-p108">**true** (указывает, что должны быть возвращены только группы безопасности, в которых состоит пользователь) и **false** (указывает, что должны быть возвращены все группы, в которых состоит пользователь). Примечание. Присвоить значение **true** можно только при вызове этого метода для пользователя.</span><span class="sxs-lookup"><span data-stu-id="93103-p108">**true** to specify that only security groups that the user is a member of should be returned; **false** to specify that all groups that the user is a member of should be returned. Note: Setting this parameter to **true** is only supported when calling this method on a user.</span></span> |

## <a name="response"></a><span data-ttu-id="93103-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="93103-145">Response</span></span>

<span data-ttu-id="93103-146">В случае успеха этот метод возвратит код отклика `200 OK` и коллекцию String в теле отклика, которое содержит идентификаторы групп, в которых состоит пользователь.</span><span class="sxs-lookup"><span data-stu-id="93103-146">If successful, this method returns `200 OK` response code and String collection in the response body that contains the IDs of the groups that the user is a member of.</span></span>

## <a name="example"></a><span data-ttu-id="93103-147">Пример</span><span class="sxs-lookup"><span data-stu-id="93103-147">Example</span></span>

<span data-ttu-id="93103-148">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="93103-148">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="93103-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="93103-149">Request</span></span>

<span data-ttu-id="93103-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="93103-150">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "user_getmembergroups"
}-->

```http
POST https://graph.microsoft.com/beta/me/getMemberGroups
Content-type: application/json
Content-length: 33

{
  "securityEnabledOnly": true
}
```

##### <a name="response"></a><span data-ttu-id="93103-151">Ответ</span><span class="sxs-lookup"><span data-stu-id="93103-151">Response</span></span>

<span data-ttu-id="93103-p109">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="93103-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
  "description": "user: getMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
