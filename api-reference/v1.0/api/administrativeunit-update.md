---
title: Обновление administrativeunit
description: Обновление свойств объекта administrativeUnit.
author: anandyadavMSFT
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 51eb82bb1bc36e5489a06feed91f34e07422fe16
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48020318"
---
# <a name="update-administrativeunit"></a><span data-ttu-id="bab8b-103">Обновление administrativeunit</span><span class="sxs-lookup"><span data-stu-id="bab8b-103">Update administrativeunit</span></span>

<span data-ttu-id="bab8b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bab8b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="bab8b-105">Обновление свойств объекта [administrativeUnit](../resources/administrativeunit.md) .</span><span class="sxs-lookup"><span data-stu-id="bab8b-105">Update the properties of an [administrativeUnit](../resources/administrativeunit.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="bab8b-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bab8b-106">Permissions</span></span>
<span data-ttu-id="bab8b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bab8b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="bab8b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bab8b-109">Permission type</span></span>      | <span data-ttu-id="bab8b-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bab8b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bab8b-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bab8b-111">Delegated (work or school account)</span></span> | <span data-ttu-id="bab8b-112">AdministrativeUnit. ReadWrite. ALL, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="bab8b-112">AdministrativeUnit.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="bab8b-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bab8b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bab8b-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bab8b-114">Not supported.</span></span>    |
|<span data-ttu-id="bab8b-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bab8b-115">Application</span></span> | <span data-ttu-id="bab8b-116">AdministrativeUnit.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bab8b-116">AdministrativeUnit.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bab8b-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bab8b-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /directory/administrativeUnits/{id}
```

## <a name="request-headers"></a><span data-ttu-id="bab8b-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bab8b-118">Request headers</span></span>

| <span data-ttu-id="bab8b-119">Имя</span><span class="sxs-lookup"><span data-stu-id="bab8b-119">Name</span></span>      |<span data-ttu-id="bab8b-120">Описание</span><span class="sxs-lookup"><span data-stu-id="bab8b-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="bab8b-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bab8b-121">Authorization</span></span>  | <span data-ttu-id="bab8b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bab8b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bab8b-124">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="bab8b-124">Request body</span></span>

<span data-ttu-id="bab8b-p103">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="bab8b-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="bab8b-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="bab8b-128">Property</span></span>   | <span data-ttu-id="bab8b-129">Тип</span><span class="sxs-lookup"><span data-stu-id="bab8b-129">Type</span></span> |<span data-ttu-id="bab8b-130">Описание</span><span class="sxs-lookup"><span data-stu-id="bab8b-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bab8b-131">description</span><span class="sxs-lookup"><span data-stu-id="bab8b-131">description</span></span>|<span data-ttu-id="bab8b-132">string</span><span class="sxs-lookup"><span data-stu-id="bab8b-132">string</span></span>|<span data-ttu-id="bab8b-133">Описание административной единицы.</span><span class="sxs-lookup"><span data-stu-id="bab8b-133">Description for the administrative unit.</span></span>|
|<span data-ttu-id="bab8b-134">displayName</span><span class="sxs-lookup"><span data-stu-id="bab8b-134">displayName</span></span>|<span data-ttu-id="bab8b-135">string</span><span class="sxs-lookup"><span data-stu-id="bab8b-135">string</span></span>|<span data-ttu-id="bab8b-136">Отображаемое имя административной единицы.</span><span class="sxs-lookup"><span data-stu-id="bab8b-136">Display name for the administrative unit.</span></span>|
|<span data-ttu-id="bab8b-137">visibility</span><span class="sxs-lookup"><span data-stu-id="bab8b-137">visibility</span></span>|<span data-ttu-id="bab8b-138">string</span><span class="sxs-lookup"><span data-stu-id="bab8b-138">string</span></span>|<span data-ttu-id="bab8b-139">Видимость административной единицы.</span><span class="sxs-lookup"><span data-stu-id="bab8b-139">Visibility for the administrative unit.</span></span> <span data-ttu-id="bab8b-140">Если не задано, то значение по умолчанию — "общедоступный".</span><span class="sxs-lookup"><span data-stu-id="bab8b-140">If not set then the default is "public".</span></span> <span data-ttu-id="bab8b-141">Может иметь значение "значение hiddenmembership", которое скрывает членство в группах, не являющихся участниками.</span><span class="sxs-lookup"><span data-stu-id="bab8b-141">Can be set to "HiddenMembership", which hides the membership from non-members.</span></span>|

<span data-ttu-id="bab8b-142">Так как ресурс **administrativeUnit** поддерживает [расширения](/graph/extensibility-overview), с помощью операции можно `PATCH` добавлять, обновлять или удалять собственные данные, зависящие от приложения, в пользовательских свойствах расширения в существующем экземпляре **administrativeUnit** .</span><span class="sxs-lookup"><span data-stu-id="bab8b-142">Since the **administrativeUnit** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **administrativeUnit** instance.</span></span>

## <a name="response"></a><span data-ttu-id="bab8b-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="bab8b-143">Response</span></span>

<span data-ttu-id="bab8b-144">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="bab8b-144">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="bab8b-145">Пример</span><span class="sxs-lookup"><span data-stu-id="bab8b-145">Example</span></span>

##### <a name="request"></a><span data-ttu-id="bab8b-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="bab8b-146">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "update_administrativeunit"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/directory/administrativeUnits/{id}
Content-type: application/json
Content-length: 114

{
  "displayName": "displayName-value",
  "description": "description-value",
  "visibility": "visibility-value"
}
```

---


##### <a name="response"></a><span data-ttu-id="bab8b-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="bab8b-147">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.administrativeunit"
} -->
```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="bab8b-148">См. также</span><span class="sxs-lookup"><span data-stu-id="bab8b-148">See also</span></span>

- [<span data-ttu-id="bab8b-149">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="bab8b-149">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="bab8b-150">Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="bab8b-150">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
<!--
- [Add custom data to groups using schema extensions (preview)](/graph/extensibility-schema-groups)
-->


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update administrativeunit",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
