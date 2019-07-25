---
title: Создание параметра каталога
description: Используйте этот API, чтобы создать новый параметр на основе шаблонов, доступных в Директорисеттингтемплатес. Эти параметры могут быть на уровне клиента или на уровне объекта (в настоящее время только для групп). Запрос на создание должен предоставлять Сеттингвалуес для всех параметров, определенных в шаблоне. Для параметров, относящихся к группе, можно задать только параметр, определяющий, могут ли участники группы приглашать гостевых пользователей. Это поведение будет управляться после того, как возможность добавлять гостей в группу является общедоступной.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: e83cff42607364ed94b9dc5aaffd8eaca950d726
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/25/2019
ms.locfileid: "35862057"
---
# <a name="create-a-directory-setting"></a><span data-ttu-id="93e00-107">Создание параметра каталога</span><span class="sxs-lookup"><span data-stu-id="93e00-107">Create a directory setting</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="93e00-108">Используйте этот API, чтобы создать новый параметр на основе шаблонов, доступных в Директорисеттингтемплатес.</span><span class="sxs-lookup"><span data-stu-id="93e00-108">Use this API to create a new setting, based on the templates available in directorySettingTemplates.</span></span> <span data-ttu-id="93e00-109">Эти параметры могут быть на уровне клиента или на уровне объекта (в настоящее время только для групп).</span><span class="sxs-lookup"><span data-stu-id="93e00-109">These settings can be at the tenant-level or at an object level (currently only for groups).</span></span> <span data-ttu-id="93e00-110">Запрос на создание должен предоставлять Сеттингвалуес для всех параметров, определенных в шаблоне.</span><span class="sxs-lookup"><span data-stu-id="93e00-110">The creation request must provide settingValues for all the settings defined in the template.</span></span> <span data-ttu-id="93e00-111">Для параметров, относящихся к группе, можно задать только параметр, определяющий, могут ли участники группы приглашать гостевых пользователей.</span><span class="sxs-lookup"><span data-stu-id="93e00-111">For group-specific settings, only the setting governing whether members of a group can invite guest users can be set.</span></span> <span data-ttu-id="93e00-112">Это поведение будет управляться после того, как возможность добавлять гостей в группу является общедоступной.</span><span class="sxs-lookup"><span data-stu-id="93e00-112">This will govern this behavior once the ability to add guest users to a group is generally available.</span></span>

> <span data-ttu-id="93e00-113">**Note**: версия/Beta этого API применяется только к группам.</span><span class="sxs-lookup"><span data-stu-id="93e00-113">**Note**: The /beta version of this API is only applies to groups.</span></span> <span data-ttu-id="93e00-114">Версия/v1.0 этого API была переименована для *создания граупсеттингс*.</span><span class="sxs-lookup"><span data-stu-id="93e00-114">The /v1.0 version of this API has been renamed to *Create groupSettings*.</span></span>

<span data-ttu-id="93e00-115">Чтобы получить список шаблонов и свойств, которые они поддерживают в бета-версии, используйте [запрос директорисеттингтемплате](https://developer.microsoft.com/graph/graph-explorer?request=directorySettingTemplates&version=beta).</span><span class="sxs-lookup"><span data-stu-id="93e00-115">For a list of templates and the properties they support in beta, use a [directorySettingTemplate query](https://developer.microsoft.com/graph/graph-explorer?request=directorySettingTemplates&version=beta).</span></span> <span data-ttu-id="93e00-116">(Для конечных точек v 1.0 вызовите [граупсеттингтемплатес](https://developer.microsoft.com/graph/graph-explorer?request=groupSettingTemplates&version=v1.0).)</span><span class="sxs-lookup"><span data-stu-id="93e00-116">(For v1.0 endpoints, call [groupSettingTemplates](https://developer.microsoft.com/graph/graph-explorer?request=groupSettingTemplates&version=v1.0).)</span></span>


## <a name="permissions"></a><span data-ttu-id="93e00-117">Разрешения</span><span class="sxs-lookup"><span data-stu-id="93e00-117">Permissions</span></span>
<span data-ttu-id="93e00-p105">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="93e00-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="93e00-120">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="93e00-120">Permission type</span></span>      | <span data-ttu-id="93e00-121">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="93e00-121">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="93e00-122">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="93e00-122">Delegated (work or school account)</span></span> | <span data-ttu-id="93e00-123">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="93e00-123">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="93e00-124">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="93e00-124">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="93e00-125">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="93e00-125">Not supported.</span></span>    |
|<span data-ttu-id="93e00-126">Для приложений</span><span class="sxs-lookup"><span data-stu-id="93e00-126">Application</span></span> | <span data-ttu-id="93e00-127">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="93e00-127">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="93e00-128">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="93e00-128">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /settings
POST /groups/{id}/settings
```
## <a name="request-headers"></a><span data-ttu-id="93e00-129">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="93e00-129">Request headers</span></span>
| <span data-ttu-id="93e00-130">Имя</span><span class="sxs-lookup"><span data-stu-id="93e00-130">Name</span></span>       | <span data-ttu-id="93e00-131">Описание</span><span class="sxs-lookup"><span data-stu-id="93e00-131">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="93e00-132">Авторизация</span><span class="sxs-lookup"><span data-stu-id="93e00-132">Authorization</span></span>  | <span data-ttu-id="93e00-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="93e00-p106">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="93e00-135">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="93e00-135">Request body</span></span>
<span data-ttu-id="93e00-136">В тексте запроса добавьте представление объекта [директорисеттинг](../resources/directorysetting.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="93e00-136">In the request body, supply a JSON representation of [directorySetting](../resources/directorysetting.md) object.</span></span>  <span data-ttu-id="93e00-137">Однако отображаемое имя для параметра будет задано на основе имени шаблона параметров, на который указывает ссылка.</span><span class="sxs-lookup"><span data-stu-id="93e00-137">However, the display name for the setting will be set based on the referenced settings template name.</span></span>

## <a name="response"></a><span data-ttu-id="93e00-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="93e00-138">Response</span></span>

<span data-ttu-id="93e00-139">В случае успешного выполнения этот метод `201 Created` возвращает код отклика и объект [директорисеттинг](../resources/directorysetting.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="93e00-139">If successful, this method returns `201 Created` response code and [directorySetting](../resources/directorysetting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="93e00-140">Пример</span><span class="sxs-lookup"><span data-stu-id="93e00-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="93e00-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="93e00-141">Request</span></span>
<span data-ttu-id="93e00-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="93e00-142">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="93e00-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="93e00-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_directorysetting_from_settings"
}-->
```http
POST https://graph.microsoft.com/beta/settings
Content-type: application/json
Content-length: 222

{
  "templateId": "templateId-value",
  "values": [
    {
      "name": "name-value",
      "value": "value-value"
    }
  ]
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="93e00-144">C#</span><span class="sxs-lookup"><span data-stu-id="93e00-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-directorysetting-from-settings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="93e00-145">Javascript</span><span class="sxs-lookup"><span data-stu-id="93e00-145">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directorysetting-from-settings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="93e00-146">Цель — C</span><span class="sxs-lookup"><span data-stu-id="93e00-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-directorysetting-from-settings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="93e00-147">Java</span><span class="sxs-lookup"><span data-stu-id="93e00-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-directorysetting-from-settings-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="93e00-148">В тексте запроса добавьте представление объекта [директорисеттинг](../resources/directorysetting.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="93e00-148">In the request body, supply a JSON representation of [directorySetting](../resources/directorysetting.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="93e00-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="93e00-149">Response</span></span>
<span data-ttu-id="93e00-p108">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="93e00-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directorySetting"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 244

{
    "@odata.context": "https://graph.microsoft.com/stagingbeta/$metadata#settings/$entity",
    "id": "id-value",
    "displayName": "displayName-value",
    "templateId": "templateId-value",
    "values": [
      {
        "name": "name-value",
        "value": "value-value"
      }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create directorySetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
