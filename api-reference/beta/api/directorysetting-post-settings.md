---
title: Создание параметра каталога
description: Используйте этот API, чтобы создать новый параметр на основе шаблонов, доступных в Директорисеттингтемплатес. Эти параметры могут быть на уровне клиента или на уровне объекта (в настоящее время только для групп). Запрос на создание должен предоставлять Сеттингвалуес для всех параметров, определенных в шаблоне. Для параметров, относящихся к группе, можно задать только параметр, определяющий, могут ли участники группы приглашать гостевых пользователей. Это поведение будет управляться после того, как возможность добавлять гостей в группу является общедоступной.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 5b88e405d8850eef49fd73fff792a94cf727863a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42433974"
---
# <a name="create-a-directory-setting"></a><span data-ttu-id="941b5-107">Создание параметра каталога</span><span class="sxs-lookup"><span data-stu-id="941b5-107">Create a directory setting</span></span>

<span data-ttu-id="941b5-108">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="941b5-108">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="941b5-109">Используйте этот API, чтобы создать новый параметр на основе шаблонов, доступных в Директорисеттингтемплатес.</span><span class="sxs-lookup"><span data-stu-id="941b5-109">Use this API to create a new setting, based on the templates available in directorySettingTemplates.</span></span> <span data-ttu-id="941b5-110">Эти параметры могут быть на уровне клиента или на уровне объекта (в настоящее время только для групп).</span><span class="sxs-lookup"><span data-stu-id="941b5-110">These settings can be at the tenant-level or at an object level (currently only for groups).</span></span> <span data-ttu-id="941b5-111">Запрос на создание должен предоставлять Сеттингвалуес для всех параметров, определенных в шаблоне.</span><span class="sxs-lookup"><span data-stu-id="941b5-111">The creation request must provide settingValues for all the settings defined in the template.</span></span> <span data-ttu-id="941b5-112">Для параметров, относящихся к группе, можно задать только параметр, определяющий, могут ли участники группы приглашать гостевых пользователей.</span><span class="sxs-lookup"><span data-stu-id="941b5-112">For group-specific settings, only the setting governing whether members of a group can invite guest users can be set.</span></span> <span data-ttu-id="941b5-113">Это поведение будет управляться после того, как возможность добавлять гостей в группу является общедоступной.</span><span class="sxs-lookup"><span data-stu-id="941b5-113">This will govern this behavior once the ability to add guest users to a group is generally available.</span></span>

> <span data-ttu-id="941b5-114">**Note**: версия/Beta этого API применяется только к группам.</span><span class="sxs-lookup"><span data-stu-id="941b5-114">**Note**: The /beta version of this API only applies to groups.</span></span> <span data-ttu-id="941b5-115">Версия/v1.0 этого API была переименована для *создания граупсеттингс*.</span><span class="sxs-lookup"><span data-stu-id="941b5-115">The /v1.0 version of this API has been renamed to *Create groupSettings*.</span></span>

<span data-ttu-id="941b5-116">Чтобы получить список шаблонов и свойств, которые они поддерживают в бета-версии, используйте [запрос директорисеттингтемплате](https://developer.microsoft.com/graph/graph-explorer?request=directorySettingTemplates&version=beta).</span><span class="sxs-lookup"><span data-stu-id="941b5-116">For a list of templates and the properties they support in beta, use a [directorySettingTemplate query](https://developer.microsoft.com/graph/graph-explorer?request=directorySettingTemplates&version=beta).</span></span> <span data-ttu-id="941b5-117">(Для конечных точек v 1.0 вызовите [граупсеттингтемплатес](https://developer.microsoft.com/graph/graph-explorer?request=groupSettingTemplates&version=v1.0).)</span><span class="sxs-lookup"><span data-stu-id="941b5-117">(For v1.0 endpoints, call [groupSettingTemplates](https://developer.microsoft.com/graph/graph-explorer?request=groupSettingTemplates&version=v1.0).)</span></span>


## <a name="permissions"></a><span data-ttu-id="941b5-118">Разрешения</span><span class="sxs-lookup"><span data-stu-id="941b5-118">Permissions</span></span>
<span data-ttu-id="941b5-p105">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="941b5-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="941b5-121">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="941b5-121">Permission type</span></span>      | <span data-ttu-id="941b5-122">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="941b5-122">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="941b5-123">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="941b5-123">Delegated (work or school account)</span></span> | <span data-ttu-id="941b5-124">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="941b5-124">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="941b5-125">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="941b5-125">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="941b5-126">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="941b5-126">Not supported.</span></span>    |
|<span data-ttu-id="941b5-127">Для приложений</span><span class="sxs-lookup"><span data-stu-id="941b5-127">Application</span></span> | <span data-ttu-id="941b5-128">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="941b5-128">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="941b5-129">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="941b5-129">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /settings
POST /groups/{id}/settings
```
## <a name="request-headers"></a><span data-ttu-id="941b5-130">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="941b5-130">Request headers</span></span>
| <span data-ttu-id="941b5-131">Имя</span><span class="sxs-lookup"><span data-stu-id="941b5-131">Name</span></span>       | <span data-ttu-id="941b5-132">Описание</span><span class="sxs-lookup"><span data-stu-id="941b5-132">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="941b5-133">Авторизация</span><span class="sxs-lookup"><span data-stu-id="941b5-133">Authorization</span></span>  | <span data-ttu-id="941b5-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="941b5-p106">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="941b5-136">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="941b5-136">Request body</span></span>
<span data-ttu-id="941b5-137">В тексте запроса добавьте представление объекта [директорисеттинг](../resources/directorysetting.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="941b5-137">In the request body, supply a JSON representation of [directorySetting](../resources/directorysetting.md) object.</span></span>  <span data-ttu-id="941b5-138">Однако отображаемое имя для параметра будет задано на основе имени шаблона параметров, на который указывает ссылка.</span><span class="sxs-lookup"><span data-stu-id="941b5-138">However, the display name for the setting will be set based on the referenced settings template name.</span></span>

## <a name="response"></a><span data-ttu-id="941b5-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="941b5-139">Response</span></span>

<span data-ttu-id="941b5-140">В случае успешного выполнения этот метод `201 Created` возвращает код отклика и объект [директорисеттинг](../resources/directorysetting.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="941b5-140">If successful, this method returns `201 Created` response code and [directorySetting](../resources/directorysetting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="941b5-141">Пример</span><span class="sxs-lookup"><span data-stu-id="941b5-141">Example</span></span>
##### <a name="request"></a><span data-ttu-id="941b5-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="941b5-142">Request</span></span>
<span data-ttu-id="941b5-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="941b5-143">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="941b5-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="941b5-144">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="941b5-145">C#</span><span class="sxs-lookup"><span data-stu-id="941b5-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-directorysetting-from-settings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="941b5-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="941b5-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directorysetting-from-settings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="941b5-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="941b5-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-directorysetting-from-settings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="941b5-148">В тексте запроса добавьте представление объекта [директорисеттинг](../resources/directorysetting.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="941b5-148">In the request body, supply a JSON representation of [directorySetting](../resources/directorysetting.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="941b5-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="941b5-149">Response</span></span>
<span data-ttu-id="941b5-p108">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="941b5-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
