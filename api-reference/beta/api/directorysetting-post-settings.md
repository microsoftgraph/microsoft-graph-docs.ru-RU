---
title: Создание параметра каталога
description: Используйте этот API, чтобы создать новый параметр на основе шаблонов, доступных в Директорисеттингтемплатес.
localization_priority: Normal
author: adimitui
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: d2a94361ee3d92ae6662751a633176ff236819ca
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48956191"
---
# <a name="create-a-directory-setting"></a><span data-ttu-id="47a49-103">Создание параметра каталога</span><span class="sxs-lookup"><span data-stu-id="47a49-103">Create a directory setting</span></span>

<span data-ttu-id="47a49-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="47a49-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="47a49-105">Используйте этот API, чтобы создать новый параметр на основе шаблонов, доступных в Директорисеттингтемплатес.</span><span class="sxs-lookup"><span data-stu-id="47a49-105">Use this API to create a new setting, based on the templates available in directorySettingTemplates.</span></span> <span data-ttu-id="47a49-106">Эти параметры могут быть на уровне клиента или на уровне объекта (в настоящее время только для групп).</span><span class="sxs-lookup"><span data-stu-id="47a49-106">These settings can be at the tenant-level or at an object level (currently only for groups).</span></span> <span data-ttu-id="47a49-107">Запрос на создание должен предоставлять Сеттингвалуес для всех параметров, определенных в шаблоне.</span><span class="sxs-lookup"><span data-stu-id="47a49-107">The creation request must provide settingValues for all the settings defined in the template.</span></span> <span data-ttu-id="47a49-108">Для параметров, относящихся к группе, можно задать только параметр, определяющий, могут ли участники группы приглашать гостевых пользователей.</span><span class="sxs-lookup"><span data-stu-id="47a49-108">For group-specific settings, only the setting governing whether members of a group can invite guest users can be set.</span></span> <span data-ttu-id="47a49-109">Это поведение будет управляться после того, как возможность добавлять гостей в группу является общедоступной.</span><span class="sxs-lookup"><span data-stu-id="47a49-109">This will govern this behavior once the ability to add guest users to a group is generally available.</span></span>

> <span data-ttu-id="47a49-110">**Note** : версия/Beta этого API применяется только к группам.</span><span class="sxs-lookup"><span data-stu-id="47a49-110">**Note** : The /beta version of this API only applies to groups.</span></span> <span data-ttu-id="47a49-111">Версия/v1.0 этого API была переименована для *создания граупсеттингс*.</span><span class="sxs-lookup"><span data-stu-id="47a49-111">The /v1.0 version of this API has been renamed to *Create groupSettings*.</span></span>

<span data-ttu-id="47a49-112">Чтобы получить список шаблонов и свойств, которые они поддерживают в бета-версии, используйте [запрос директорисеттингтемплате](https://developer.microsoft.com/graph/graph-explorer?request=directorySettingTemplates&version=beta).</span><span class="sxs-lookup"><span data-stu-id="47a49-112">For a list of templates and the properties they support in beta, use a [directorySettingTemplate query](https://developer.microsoft.com/graph/graph-explorer?request=directorySettingTemplates&version=beta).</span></span> <span data-ttu-id="47a49-113">(Для конечных точек v 1.0 вызовите [граупсеттингтемплатес](https://developer.microsoft.com/graph/graph-explorer?request=groupSettingTemplates&version=v1.0).)</span><span class="sxs-lookup"><span data-stu-id="47a49-113">(For v1.0 endpoints, call [groupSettingTemplates](https://developer.microsoft.com/graph/graph-explorer?request=groupSettingTemplates&version=v1.0).)</span></span>


## <a name="permissions"></a><span data-ttu-id="47a49-114">Разрешения</span><span class="sxs-lookup"><span data-stu-id="47a49-114">Permissions</span></span>
<span data-ttu-id="47a49-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="47a49-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="47a49-117">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="47a49-117">Permission type</span></span>      | <span data-ttu-id="47a49-118">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="47a49-118">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="47a49-119">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="47a49-119">Delegated (work or school account)</span></span> | <span data-ttu-id="47a49-120">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="47a49-120">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="47a49-121">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="47a49-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="47a49-122">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="47a49-122">Not supported.</span></span>    |
|<span data-ttu-id="47a49-123">Для приложений</span><span class="sxs-lookup"><span data-stu-id="47a49-123">Application</span></span> | <span data-ttu-id="47a49-124">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="47a49-124">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="47a49-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="47a49-125">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /settings
POST /groups/{id}/settings
```
## <a name="request-headers"></a><span data-ttu-id="47a49-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="47a49-126">Request headers</span></span>
| <span data-ttu-id="47a49-127">Имя</span><span class="sxs-lookup"><span data-stu-id="47a49-127">Name</span></span>       | <span data-ttu-id="47a49-128">Описание</span><span class="sxs-lookup"><span data-stu-id="47a49-128">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="47a49-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="47a49-129">Authorization</span></span>  | <span data-ttu-id="47a49-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="47a49-p105">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="47a49-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="47a49-132">Request body</span></span>
<span data-ttu-id="47a49-133">В тексте запроса добавьте представление объекта [директорисеттинг](../resources/directorysetting.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="47a49-133">In the request body, supply a JSON representation of [directorySetting](../resources/directorysetting.md) object.</span></span>  <span data-ttu-id="47a49-134">Однако отображаемое имя для параметра будет задано на основе имени шаблона параметров, на который указывает ссылка.</span><span class="sxs-lookup"><span data-stu-id="47a49-134">However, the display name for the setting will be set based on the referenced settings template name.</span></span>

## <a name="response"></a><span data-ttu-id="47a49-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="47a49-135">Response</span></span>

<span data-ttu-id="47a49-136">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [директорисеттинг](../resources/directorysetting.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="47a49-136">If successful, this method returns `201 Created` response code and [directorySetting](../resources/directorysetting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="47a49-137">Пример</span><span class="sxs-lookup"><span data-stu-id="47a49-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="47a49-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="47a49-138">Request</span></span>
<span data-ttu-id="47a49-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="47a49-139">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="47a49-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="47a49-140">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="47a49-141">C#</span><span class="sxs-lookup"><span data-stu-id="47a49-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-directorysetting-from-settings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="47a49-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="47a49-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directorysetting-from-settings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="47a49-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="47a49-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-directorysetting-from-settings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="47a49-144">Java</span><span class="sxs-lookup"><span data-stu-id="47a49-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-directorysetting-from-settings-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="47a49-145">В тексте запроса добавьте представление объекта [директорисеттинг](../resources/directorysetting.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="47a49-145">In the request body, supply a JSON representation of [directorySetting](../resources/directorysetting.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="47a49-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="47a49-146">Response</span></span>
<span data-ttu-id="47a49-p107">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="47a49-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


