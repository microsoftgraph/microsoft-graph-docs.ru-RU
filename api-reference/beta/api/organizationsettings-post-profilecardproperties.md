---
title: Создание Профилекардпроперти
description: Используйте этот API для создания нового Профилекардпроперти.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 24fe1a2f4257475849ecb3c057843d7cd0661a21
ms.sourcegitcommit: 2050639c9e9a6b2dab9ce53d6a9fc87e98789b50
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/08/2020
ms.locfileid: "45080641"
---
# <a name="create-profilecardproperty"></a><span data-ttu-id="c586a-103">Создание Профилекардпроперти</span><span class="sxs-lookup"><span data-stu-id="c586a-103">Create profileCardProperty</span></span>

<span data-ttu-id="c586a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c586a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c586a-105">Создание нового [профилекардпроперти](../resources/profilecardproperty.md) для Организации.</span><span class="sxs-lookup"><span data-stu-id="c586a-105">Create a new [profileCardProperty](../resources/profilecardproperty.md) for an organization.</span></span> <span data-ttu-id="c586a-106">Новое свойство определяется свойством **директорипропертинаме** .</span><span class="sxs-lookup"><span data-stu-id="c586a-106">The new property is identified by its **directoryPropertyName** property.</span></span>

<span data-ttu-id="c586a-107">Дополнительные сведения о добавлении свойств в карточку профиля для организации можно узнать в статье [Настройка карточки профиля](/graph/add-properties-profilecard).</span><span class="sxs-lookup"><span data-stu-id="c586a-107">For more information on adding properties to the profile card for an organization, see [customize the profile card](/graph/add-properties-profilecard).</span></span>

## <a name="permissions"></a><span data-ttu-id="c586a-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c586a-108">Permissions</span></span>

<span data-ttu-id="c586a-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="c586a-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="c586a-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c586a-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c586a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c586a-111">Permission type</span></span>                        | <span data-ttu-id="c586a-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c586a-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="c586a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c586a-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="c586a-114">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="c586a-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="c586a-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c586a-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c586a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c586a-116">Not supported.</span></span>                              |
| <span data-ttu-id="c586a-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c586a-117">Application</span></span>                            | <span data-ttu-id="c586a-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c586a-118">Not supported.</span></span>                              |

><span data-ttu-id="c586a-119">**Примечание:** Для этой операции с делегированными разрешениями необходимо, чтобы вошедшего в систему пользователя была назначена роль администратора клиента или роль глобального администратора.</span><span class="sxs-lookup"><span data-stu-id="c586a-119">**Note:** Using delegated permissions for this operation requires the signed-in user to have a tenant administrator or global administrator role.</span></span>

## <a name="http-request"></a><span data-ttu-id="c586a-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c586a-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST https://graph.microsoft.com/beta/organization/settings/profileCardProperties
```

## <a name="request-headers"></a><span data-ttu-id="c586a-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c586a-121">Request headers</span></span>

| <span data-ttu-id="c586a-122">Имя</span><span class="sxs-lookup"><span data-stu-id="c586a-122">Name</span></span>          |<span data-ttu-id="c586a-123">Описание</span><span class="sxs-lookup"><span data-stu-id="c586a-123">Description</span></span>                  |
|:--------------|:----------------------------|
| <span data-ttu-id="c586a-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c586a-124">Authorization</span></span> | <span data-ttu-id="c586a-125">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="c586a-125">Bearer {token}.</span></span> <span data-ttu-id="c586a-126">Required.</span><span class="sxs-lookup"><span data-stu-id="c586a-126">Required.</span></span>   |
| <span data-ttu-id="c586a-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c586a-127">Content-Type</span></span>  | <span data-ttu-id="c586a-128">application/json.</span><span class="sxs-lookup"><span data-stu-id="c586a-128">application/json.</span></span> <span data-ttu-id="c586a-129">Required.</span><span class="sxs-lookup"><span data-stu-id="c586a-129">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c586a-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c586a-130">Request body</span></span>

<span data-ttu-id="c586a-131">В тексте запроса добавьте представление объекта [профилекардпроперти](../resources/profilecardproperty.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c586a-131">In the request body, supply a JSON representation of a [profileCardProperty](../resources/profilecardproperty.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="c586a-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="c586a-132">Response</span></span>

<span data-ttu-id="c586a-133">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и новый объект [профилекардпроперти](../resources/profilecardproperty.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c586a-133">If successful, this method returns `201 Created` response code and a new [profileCardProperty](../resources/profilecardproperty.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c586a-134">Примеры</span><span class="sxs-lookup"><span data-stu-id="c586a-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c586a-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="c586a-135">Request</span></span>

<span data-ttu-id="c586a-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c586a-136">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c586a-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="c586a-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_profilecardproperty_from_organizationsettings"
}-->

```http
POST https://graph.microsoft.com/beta/organization/settings/profileCardProperties
Content-type: application/json

{
  "directoryPropertyName": "CustomAttribute1",
  "annotations": [
    {
      "displayName": "Cost Center",
      "localizations": [
        {
          "languageTag": "ru-RU",
          "displayName": "центр затрат"
        }
      ]
    }
  ]
}
```
# <a name="javascript"></a>[<span data-ttu-id="c586a-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c586a-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-profilecardproperty-from-organizationsettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c586a-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="c586a-139">Response</span></span>

<span data-ttu-id="c586a-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c586a-140">The following is an example of the response.</span></span>

> <span data-ttu-id="c586a-141">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="c586a-141">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="c586a-142">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="c586a-142">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.profileCardProperty"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "directoryPropertyName": "CustomAttribute1",
  "annotations": [
    {
      "displayName": "Cost Center",
      "localizations": [
        {
          "languageTag": "ru-RU",
          "displayName": "центр затрат"
        }
      ]
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create profileCardProperty",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
