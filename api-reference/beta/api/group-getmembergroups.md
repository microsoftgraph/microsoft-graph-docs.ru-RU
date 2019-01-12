---
title: 'group: getMemberGroups'
description: Возвращает все названия групп, в которых состоит указанная группа. Эта промежуточная проверка, в отличие от считывания свойства навигации memberOf (возвращаются только группы, непосредственным членом которых является данная группа).
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: e485c80a06fc2d124dec728ab3ffcdfb8dcce105
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27921537"
---
# <a name="group-getmembergroups"></a><span data-ttu-id="18453-104">group: getMemberGroups</span><span class="sxs-lookup"><span data-stu-id="18453-104">group: getMemberGroups</span></span>

> <span data-ttu-id="18453-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="18453-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="18453-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="18453-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="18453-p103">Возвращает все названия групп, в которых состоит указанная группа. Эта промежуточная проверка, в отличие от считывания свойства навигации [memberOf](../api/group-list-memberof.md) (возвращаются только группы, непосредственным членом которых является данная группа).</span><span class="sxs-lookup"><span data-stu-id="18453-p103">Return all the groups that the specified group is a member of. The check is transitive, unlike reading the [memberOf](../api/group-list-memberof.md) navigation property, which returns only the groups that the group is a direct member of.</span></span>

<span data-ttu-id="18453-p104">Эта функция поддерживает Office 365 и другие типы групп, подготовленных к работе в Azure AD. Максимальное количество групп, которые может вернуть каждый запрос, — 2046. Обратите внимание, что компонент "Группы Office 365" не может содержать группы. Следовательно, членство, относящееся к компоненту "Группы Office 365", всегда непосредственное.</span><span class="sxs-lookup"><span data-stu-id="18453-p104">This function supports Office 365 and other types of groups provisioned in Azure AD. The maximum number of groups each request can return is 2046. Note that Office 365 Groups cannot contain groups. So membership in an Office 365 Group is always direct.</span></span>

## <a name="permissions"></a><span data-ttu-id="18453-113">Разрешения</span><span class="sxs-lookup"><span data-stu-id="18453-113">Permissions</span></span>

<span data-ttu-id="18453-p105">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="18453-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="18453-116">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="18453-116">Permission type</span></span>                        | <span data-ttu-id="18453-117">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="18453-117">Permissions (from least to most privileged)</span></span>                                                 |
| :------------------------------------- | :------------------------------------------------------------------------------------------ |
| <span data-ttu-id="18453-118">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="18453-118">Delegated (work or school account)</span></span>     | <span data-ttu-id="18453-119">~~Group.Read.All~~, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="18453-119">~~Group.Read.All~~, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="18453-120">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="18453-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="18453-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="18453-121">Not supported.</span></span>                                                                              |
| <span data-ttu-id="18453-122">Для приложения</span><span class="sxs-lookup"><span data-stu-id="18453-122">Application</span></span>                            | <span data-ttu-id="18453-123">~~Group.Read.All~~, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18453-123">~~Group.Read.All~~, Directory.Read.All, Directory.ReadWrite.All</span></span>                             |

> <span data-ttu-id="18453-124">**Примечание:** Этот интерфейс API в настоящее время требует `Directory.Read.All` разрешений или выше.</span><span class="sxs-lookup"><span data-stu-id="18453-124">**Note:** This API currently requires the `Directory.Read.All` permission or higher.</span></span> <span data-ttu-id="18453-125">С помощью `Group.Read.All` разрешение возвращает ошибку.</span><span class="sxs-lookup"><span data-stu-id="18453-125">Using the `Group.Read.All` permission will return an error.</span></span> <span data-ttu-id="18453-126">Мы знаем об этой проблеме.</span><span class="sxs-lookup"><span data-stu-id="18453-126">This is a known bug.</span></span>

## <a name="http-request"></a><span data-ttu-id="18453-127">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="18453-127">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /groups/{id}/getMemberGroups
```

## <a name="request-headers"></a><span data-ttu-id="18453-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="18453-128">Request headers</span></span>

| <span data-ttu-id="18453-129">Имя</span><span class="sxs-lookup"><span data-stu-id="18453-129">Name</span></span>          | <span data-ttu-id="18453-130">Тип</span><span class="sxs-lookup"><span data-stu-id="18453-130">Type</span></span>   | <span data-ttu-id="18453-131">Описание</span><span class="sxs-lookup"><span data-stu-id="18453-131">Description</span></span>               |
| :------------ | :----- | :------------------------ |
| <span data-ttu-id="18453-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="18453-132">Authorization</span></span> | <span data-ttu-id="18453-133">строка</span><span class="sxs-lookup"><span data-stu-id="18453-133">string</span></span> | <span data-ttu-id="18453-p107">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="18453-p107">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="18453-136">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="18453-136">Request body</span></span>

<span data-ttu-id="18453-137">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="18453-137">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="18453-138">Параметр</span><span class="sxs-lookup"><span data-stu-id="18453-138">Parameter</span></span>           | <span data-ttu-id="18453-139">Тип</span><span class="sxs-lookup"><span data-stu-id="18453-139">Type</span></span>    | <span data-ttu-id="18453-140">Описание</span><span class="sxs-lookup"><span data-stu-id="18453-140">Description</span></span>                                                                           |
| :------------------ | :------ | :------------------------------------------------------------------------------------ |
| <span data-ttu-id="18453-141">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="18453-141">securityEnabledOnly</span></span> | <span data-ttu-id="18453-142">Логическое</span><span class="sxs-lookup"><span data-stu-id="18453-142">Boolean</span></span> | <span data-ttu-id="18453-p108">Задано значение **false**. Возвращение лишь защищенных групп поддерживается только для пользователей.</span><span class="sxs-lookup"><span data-stu-id="18453-p108">Set to **false**. Returning only security-enabled groups is supported for users only.</span></span> |

## <a name="response"></a><span data-ttu-id="18453-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="18453-145">Response</span></span>

<span data-ttu-id="18453-146">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию String в тексте отклика, содержащем идентификаторы групп, в которых состоит данная группа.</span><span class="sxs-lookup"><span data-stu-id="18453-146">If successful, this method returns `200 OK` response code and String collection in the response body that contains the IDs of the groups that the group is a member of.</span></span>

## <a name="example"></a><span data-ttu-id="18453-147">Пример</span><span class="sxs-lookup"><span data-stu-id="18453-147">Example</span></span>

#### <a name="request"></a><span data-ttu-id="18453-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="18453-148">Request</span></span>

<span data-ttu-id="18453-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="18453-149">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "group_getmembergroups"
}-->

```http
POST https://graph.microsoft.com/beta/groups/{id}/getMemberGroups
Content-type: application/json
Content-length: 33

{
  "securityEnabledOnly": false
}
```

#### <a name="response"></a><span data-ttu-id="18453-150">Ответ</span><span class="sxs-lookup"><span data-stu-id="18453-150">Response</span></span>

<span data-ttu-id="18453-151">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="18453-151">The following is an example of the response.</span></span>

> <span data-ttu-id="18453-p109">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="18453-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "description": "group: getMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
