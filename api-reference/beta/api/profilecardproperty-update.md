---
title: Обновление profileCardProperty
description: Обновление свойств объекта Профилекардпроперти.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 122b8c0007067dafd2f7326cffc1b4e3b1697890
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/14/2020
ms.locfileid: "45123857"
---
# <a name="update-profilecardproperty"></a><span data-ttu-id="5be3b-103">Обновление profileCardProperty</span><span class="sxs-lookup"><span data-stu-id="5be3b-103">Update profileCardProperty</span></span>

<span data-ttu-id="5be3b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5be3b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5be3b-105">Обновление свойств объекта [профилекардпроперти](../resources/profilecardproperty.md) , идентифицируемого его свойством **директорипропертинаме** .</span><span class="sxs-lookup"><span data-stu-id="5be3b-105">Update the properties of a [profileCardProperty](../resources/profilecardproperty.md) object, identified by its **directoryPropertyName** property.</span></span>

## <a name="permissions"></a><span data-ttu-id="5be3b-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5be3b-106">Permissions</span></span>

<span data-ttu-id="5be3b-107">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="5be3b-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="5be3b-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5be3b-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5be3b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5be3b-109">Permission type</span></span>                        | <span data-ttu-id="5be3b-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5be3b-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="5be3b-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5be3b-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="5be3b-112">User. ReadWrite, User. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="5be3b-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="5be3b-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5be3b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5be3b-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5be3b-114">Not supported.</span></span>                              |
| <span data-ttu-id="5be3b-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5be3b-115">Application</span></span>                            | <span data-ttu-id="5be3b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5be3b-116">Not supported.</span></span>                              |

><span data-ttu-id="5be3b-117">**Примечание:** Для этой операции с делегированными разрешениями необходимо, чтобы вошедшего в систему пользователя была назначена роль администратора клиента или роль глобального администратора.</span><span class="sxs-lookup"><span data-stu-id="5be3b-117">**Note:** Using delegated permissions for this operation requires the signed-in user to have a tenant administrator or global administrator role.</span></span>

## <a name="http-request"></a><span data-ttu-id="5be3b-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5be3b-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH https://graph.microsoft.com/beta/organization/{organizationId}/settings/profileCardProperties/{id}
```

## <a name="request-headers"></a><span data-ttu-id="5be3b-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5be3b-119">Request headers</span></span>

| <span data-ttu-id="5be3b-120">Имя</span><span class="sxs-lookup"><span data-stu-id="5be3b-120">Name</span></span>       | <span data-ttu-id="5be3b-121">Описание</span><span class="sxs-lookup"><span data-stu-id="5be3b-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="5be3b-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5be3b-122">Authorization</span></span> | <span data-ttu-id="5be3b-123">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="5be3b-123">Bearer {token}.</span></span> <span data-ttu-id="5be3b-124">Required.</span><span class="sxs-lookup"><span data-stu-id="5be3b-124">Required.</span></span> |
| <span data-ttu-id="5be3b-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5be3b-125">Content-Type</span></span>  | <span data-ttu-id="5be3b-126">application/json.</span><span class="sxs-lookup"><span data-stu-id="5be3b-126">application/json.</span></span> <span data-ttu-id="5be3b-127">Required.</span><span class="sxs-lookup"><span data-stu-id="5be3b-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5be3b-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5be3b-128">Request body</span></span>

<span data-ttu-id="5be3b-129">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="5be3b-129">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="5be3b-130">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="5be3b-130">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="5be3b-131">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="5be3b-131">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="5be3b-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="5be3b-132">Property</span></span>     | <span data-ttu-id="5be3b-133">Тип</span><span class="sxs-lookup"><span data-stu-id="5be3b-133">Type</span></span>        | <span data-ttu-id="5be3b-134">Описание</span><span class="sxs-lookup"><span data-stu-id="5be3b-134">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="5be3b-135">Комментарии</span><span class="sxs-lookup"><span data-stu-id="5be3b-135">annotations</span></span>|<span data-ttu-id="5be3b-136">Коллекция Профилекарданнотатион</span><span class="sxs-lookup"><span data-stu-id="5be3b-136">profileCardAnnotation collection</span></span>| <span data-ttu-id="5be3b-137">Содержит любые альтернативные или локализованные метки, которые указал Администратор.</span><span class="sxs-lookup"><span data-stu-id="5be3b-137">Contains any alternative or localized labels an administrator has chosen to specify.</span></span>|
|<span data-ttu-id="5be3b-138">директорипропертинаме</span><span class="sxs-lookup"><span data-stu-id="5be3b-138">directoryPropertyName</span></span>|<span data-ttu-id="5be3b-139">String</span><span class="sxs-lookup"><span data-stu-id="5be3b-139">String</span></span>|<span data-ttu-id="5be3b-140">Содержит имя свойства каталога, которое предназначено для отображения на карточке профиля.</span><span class="sxs-lookup"><span data-stu-id="5be3b-140">Contains the name of the directory property which is intended to surface on the profile card.</span></span> |

## <a name="response"></a><span data-ttu-id="5be3b-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="5be3b-141">Response</span></span>

<span data-ttu-id="5be3b-142">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [профилекардпроперти](../resources/profilecardproperty.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5be3b-142">If successful, this method returns a `200 OK` response code and an updated [profileCardProperty](../resources/profilecardproperty.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5be3b-143">Примеры</span><span class="sxs-lookup"><span data-stu-id="5be3b-143">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5be3b-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="5be3b-144">Request</span></span>

<span data-ttu-id="5be3b-145">В примере ниже показано, как добавить локализованную метку "Костнадс Sent" для языкового стандарта "No – NetBIOS".</span><span class="sxs-lookup"><span data-stu-id="5be3b-145">The following example adds a localized label "Kostnads Senter" for the locale "no-NB".</span></span>

# <a name="http"></a>[<span data-ttu-id="5be3b-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="5be3b-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_profilecardproperty"
}-->

```http
PATCH https://graph.microsoft.com/beta/organization/{organizationId}/settings/profileCardProperties/CustomAttribute1
Content-type: application/json

{
  "annotations": [
    {
      "localizations": [
        {
          "languageTag": "no-NB",
          "displayName": "Kostnads Senter"
        }
      ]
    }
  ]
}
```
# <a name="javascript"></a>[<span data-ttu-id="5be3b-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5be3b-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-profilecardproperty-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="5be3b-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="5be3b-148">Response</span></span>

<span data-ttu-id="5be3b-149">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="5be3b-149">The following is an example of the response.</span></span>

> <span data-ttu-id="5be3b-150">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="5be3b-150">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="5be3b-151">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="5be3b-151">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.profileCardProperty"
} -->

```http
HTTP/1.1 200 OK
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
        },
        {
          "languageTag": "no-NB",
          "displayName": "Kostnads Senter"
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
  "description": "Update profilecardproperty",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
