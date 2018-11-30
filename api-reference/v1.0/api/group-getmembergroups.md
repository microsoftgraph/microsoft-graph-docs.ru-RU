---
title: 'group: getMemberGroups'
description: Возвращает все названия групп, в которых состоит указанная группа. Эта промежуточная проверка, в отличие от считывания свойства навигации memberOf (возвращаются только группы, непосредственным членом которых является данная группа).
ms.openlocfilehash: a6778b37ef89444a47babbea8f11050e5ffcb974
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27026003"
---
# <a name="group-getmembergroups"></a><span data-ttu-id="4f5fd-104">group: getMemberGroups</span><span class="sxs-lookup"><span data-stu-id="4f5fd-104">group: getMemberGroups</span></span>

<span data-ttu-id="4f5fd-p102">Возвращает все названия групп, в которых состоит указанная группа. Эта промежуточная проверка, в отличие от считывания свойства навигации [memberOf](../api/group-list-memberof.md) (возвращаются только группы, непосредственным членом которых является данная группа).</span><span class="sxs-lookup"><span data-stu-id="4f5fd-p102">Return all the groups that the specified group is a member of. The check is transitive, unlike reading the [memberOf](../api/group-list-memberof.md) navigation property, which returns only the groups that the group is a direct member of.</span></span>

<span data-ttu-id="4f5fd-p103">Эта функция поддерживает Office 365 и другие типы групп, подготовленных к работе в Azure AD. Максимальное количество групп, которые может вернуть каждый запрос, — 2046. Обратите внимание, что компонент "Группы Office 365" не может содержать группы. Следовательно, членство, относящееся к компоненту "Группы Office 365", всегда непосредственное.</span><span class="sxs-lookup"><span data-stu-id="4f5fd-p103">This function supports Office 365 and other types of groups provisioned in Azure AD. The maximum number of groups each request can return is 2046. Note that Office 365 Groups cannot contain groups. So membership in an Office 365 Group is always direct.</span></span>

## <a name="permissions"></a><span data-ttu-id="4f5fd-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4f5fd-111">Permissions</span></span>

<span data-ttu-id="4f5fd-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4f5fd-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4f5fd-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4f5fd-114">Permission type</span></span>                        | <span data-ttu-id="4f5fd-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4f5fd-115">Permissions (from least to most privileged)</span></span>                                                 |
| :------------------------------------- | :------------------------------------------------------------------------------------------ |
| <span data-ttu-id="4f5fd-116">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4f5fd-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="4f5fd-117">~~Group.Read.All~~, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="4f5fd-117">~~Group.Read.All~~, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="4f5fd-118">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4f5fd-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4f5fd-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4f5fd-119">Not supported.</span></span>                                                                              |
| <span data-ttu-id="4f5fd-120">Для приложения</span><span class="sxs-lookup"><span data-stu-id="4f5fd-120">Application</span></span>                            | <span data-ttu-id="4f5fd-121">~~Group.Read.All~~, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4f5fd-121">~~Group.Read.All~~, Directory.Read.All, Directory.ReadWrite.All</span></span>                             |

> <span data-ttu-id="4f5fd-122">**Примечание:** Этот интерфейс API в настоящее время требует `Directory.Read.All` разрешений или выше.</span><span class="sxs-lookup"><span data-stu-id="4f5fd-122">**Note:** This API currently requires the `Directory.Read.All` permission or higher.</span></span> <span data-ttu-id="4f5fd-123">С помощью `Group.Read.All` разрешение возвращает ошибку.</span><span class="sxs-lookup"><span data-stu-id="4f5fd-123">Using the `Group.Read.All` permission will return an error.</span></span> <span data-ttu-id="4f5fd-124">Мы знаем об этой проблеме.</span><span class="sxs-lookup"><span data-stu-id="4f5fd-124">This is a known bug.</span></span>

## <a name="http-request"></a><span data-ttu-id="4f5fd-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4f5fd-125">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /groups/{id}/getMemberGroups
```

## <a name="request-headers"></a><span data-ttu-id="4f5fd-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4f5fd-126">Request headers</span></span>

| <span data-ttu-id="4f5fd-127">Имя</span><span class="sxs-lookup"><span data-stu-id="4f5fd-127">Name</span></span>          | <span data-ttu-id="4f5fd-128">Тип</span><span class="sxs-lookup"><span data-stu-id="4f5fd-128">Type</span></span>   | <span data-ttu-id="4f5fd-129">Описание</span><span class="sxs-lookup"><span data-stu-id="4f5fd-129">Description</span></span>               |
| :------------ | :----- | :------------------------ |
| <span data-ttu-id="4f5fd-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="4f5fd-130">Authorization</span></span> | <span data-ttu-id="4f5fd-131">string</span><span class="sxs-lookup"><span data-stu-id="4f5fd-131">string</span></span> | <span data-ttu-id="4f5fd-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4f5fd-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4f5fd-134">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4f5fd-134">Request body</span></span>

<span data-ttu-id="4f5fd-135">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="4f5fd-135">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="4f5fd-136">Параметр</span><span class="sxs-lookup"><span data-stu-id="4f5fd-136">Parameter</span></span>           | <span data-ttu-id="4f5fd-137">Тип</span><span class="sxs-lookup"><span data-stu-id="4f5fd-137">Type</span></span>    | <span data-ttu-id="4f5fd-138">Описание</span><span class="sxs-lookup"><span data-stu-id="4f5fd-138">Description</span></span>                                                                           |
| :------------------ | :------ | :------------------------------------------------------------------------------------ |
| <span data-ttu-id="4f5fd-139">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="4f5fd-139">securityEnabledOnly</span></span> | <span data-ttu-id="4f5fd-140">Логическое</span><span class="sxs-lookup"><span data-stu-id="4f5fd-140">Boolean</span></span> | <span data-ttu-id="4f5fd-p107">Задано значение **false**. Возвращение лишь защищенных групп поддерживается только для пользователей.</span><span class="sxs-lookup"><span data-stu-id="4f5fd-p107">Set to **false**. Returning only security-enabled groups is supported for users only.</span></span> |

## <a name="response"></a><span data-ttu-id="4f5fd-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="4f5fd-143">Response</span></span>

<span data-ttu-id="4f5fd-144">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию String в тексте отклика, содержащем идентификаторы групп, в которых состоит данная группа.</span><span class="sxs-lookup"><span data-stu-id="4f5fd-144">If successful, this method returns `200 OK` response code and String collection in the response body that contains the IDs of the groups that the group is a member of.</span></span>

## <a name="example"></a><span data-ttu-id="4f5fd-145">Пример</span><span class="sxs-lookup"><span data-stu-id="4f5fd-145">Example</span></span>

#### <a name="request"></a><span data-ttu-id="4f5fd-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="4f5fd-146">Request</span></span>

<span data-ttu-id="4f5fd-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4f5fd-147">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "group_getmembergroups"
}-->

```http
POST https://graph.microsoft.com/v1.0/groups/{id}/getMemberGroups
Content-type: application/json
Content-length: 33

{
  "securityEnabledOnly": false
}
```

#### <a name="response"></a><span data-ttu-id="4f5fd-148">Ответ</span><span class="sxs-lookup"><span data-stu-id="4f5fd-148">Response</span></span>

<span data-ttu-id="4f5fd-149">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="4f5fd-149">The following is an example of the response.</span></span>

> <span data-ttu-id="4f5fd-150">**Примечание:** объект ответа, показанный здесь может быть сокращение для удобства чтения.</span><span class="sxs-lookup"><span data-stu-id="4f5fd-150">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="4f5fd-151">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4f5fd-151">All the properties will be returned from an actual call.</span></span>

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
