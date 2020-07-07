---
title: Создание Профилекардпроперти
description: Используйте этот API для создания нового Профилекардпроперти.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 1bbdb77ea7d9cd9d76f63198b449b4f03181bc62
ms.sourcegitcommit: 67433748b69541727185fc1f32ed356718bf6ff1
ms.contentlocale: ru-RU
ms.lasthandoff: 07/07/2020
ms.locfileid: "45051134"
---
# <a name="create-profilecardproperty"></a><span data-ttu-id="469c4-103">Создание Профилекардпроперти</span><span class="sxs-lookup"><span data-stu-id="469c4-103">Create profileCardProperty</span></span>

<span data-ttu-id="469c4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="469c4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="469c4-105">Создание нового [профилекардпроперти](../resources/profilecardproperty.md) для Организации.</span><span class="sxs-lookup"><span data-stu-id="469c4-105">Create a new [profileCardProperty](../resources/profilecardproperty.md) for an organization.</span></span> <span data-ttu-id="469c4-106">Новое свойство определяется свойством **директорипропертинаме** .</span><span class="sxs-lookup"><span data-stu-id="469c4-106">The new property is identified by its **directoryPropertyName** property.</span></span>

<span data-ttu-id="469c4-107">Дополнительные сведения о добавлении свойств в карточку профиля для организации можно узнать в статье Настройка карточки профиля.</span><span class="sxs-lookup"><span data-stu-id="469c4-107">For more information on adding properties to the profile card for an organization, see customize the profile card.</span></span>

## <a name="permissions"></a><span data-ttu-id="469c4-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="469c4-108">Permissions</span></span>

<span data-ttu-id="469c4-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="469c4-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="469c4-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="469c4-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="469c4-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="469c4-111">Permission type</span></span>                        | <span data-ttu-id="469c4-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="469c4-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="469c4-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="469c4-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="469c4-114">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="469c4-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="469c4-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="469c4-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="469c4-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="469c4-116">Not supported.</span></span>                              |
| <span data-ttu-id="469c4-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="469c4-117">Application</span></span>                            | <span data-ttu-id="469c4-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="469c4-118">Not supported.</span></span>                              |

><span data-ttu-id="469c4-119">**Примечание:** Для этой операции с делегированными разрешениями необходимо, чтобы вошедшего в систему пользователя была назначена роль администратора клиента или роль глобального администратора.</span><span class="sxs-lookup"><span data-stu-id="469c4-119">**Note:** Using delegated permissions for this operation requires the signed-in user to have a tenant administrator or global administrator role.</span></span>

## <a name="http-request"></a><span data-ttu-id="469c4-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="469c4-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST https://graph.microsoft.com/beta/organization/settings/profileCardProperties
```

## <a name="request-headers"></a><span data-ttu-id="469c4-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="469c4-121">Request headers</span></span>

| <span data-ttu-id="469c4-122">Имя</span><span class="sxs-lookup"><span data-stu-id="469c4-122">Name</span></span>          |<span data-ttu-id="469c4-123">Описание</span><span class="sxs-lookup"><span data-stu-id="469c4-123">Description</span></span>                  |
|:--------------|:----------------------------|
| <span data-ttu-id="469c4-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="469c4-124">Authorization</span></span> | <span data-ttu-id="469c4-125">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="469c4-125">Bearer {token}.</span></span> <span data-ttu-id="469c4-126">Required.</span><span class="sxs-lookup"><span data-stu-id="469c4-126">Required.</span></span>   |
| <span data-ttu-id="469c4-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="469c4-127">Content-Type</span></span>  | <span data-ttu-id="469c4-128">application/json.</span><span class="sxs-lookup"><span data-stu-id="469c4-128">application/json.</span></span> <span data-ttu-id="469c4-129">Required.</span><span class="sxs-lookup"><span data-stu-id="469c4-129">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="469c4-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="469c4-130">Request body</span></span>

<span data-ttu-id="469c4-131">В тексте запроса добавьте представление объекта [профилекардпроперти](../resources/profilecardproperty.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="469c4-131">In the request body, supply a JSON representation of a [profileCardProperty](../resources/profilecardproperty.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="469c4-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="469c4-132">Response</span></span>

<span data-ttu-id="469c4-133">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и новый объект [профилекардпроперти](../resources/profilecardproperty.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="469c4-133">If successful, this method returns `201 Created` response code and a new [profileCardProperty](../resources/profilecardproperty.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="469c4-134">Примеры</span><span class="sxs-lookup"><span data-stu-id="469c4-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="469c4-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="469c4-135">Request</span></span>

<span data-ttu-id="469c4-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="469c4-136">The following is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="469c4-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="469c4-137">Response</span></span>

<span data-ttu-id="469c4-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="469c4-138">The following is an example of the response.</span></span>

> <span data-ttu-id="469c4-139">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="469c4-139">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="469c4-140">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="469c4-140">All the properties will be returned from an actual call.</span></span>

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
