---
title: Создайте параметр каталога
description: Используйте этот интерфейс API для создания нового параметра, на основе шаблонов, доступных в directorySettingTemplates. Эти параметры можно на уровне клиента или на уровне объекта (в настоящее время только для групп). Запрос на создание необходимо задать settingValues для всех параметров, определенных в шаблоне. Для определенных параметров может устанавливаться только параметр Управление ли членов группы можно приглашать пользователей гостя. Преимущественную это поведение после общедоступной возможность добавления гостевых пользователей в группу.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: f74c449f02726adc4ba0993f450a8a4351ec8f2a
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29520755"
---
# <a name="create-a-directory-setting"></a><span data-ttu-id="f8769-107">Создайте параметр каталога</span><span class="sxs-lookup"><span data-stu-id="f8769-107">Create a directory setting</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f8769-108">Используйте этот интерфейс API для создания нового параметра, на основе шаблонов, доступных в directorySettingTemplates.</span><span class="sxs-lookup"><span data-stu-id="f8769-108">Use this API to create a new setting, based on the templates available in directorySettingTemplates.</span></span> <span data-ttu-id="f8769-109">Эти параметры можно на уровне клиента или на уровне объекта (в настоящее время только для групп).</span><span class="sxs-lookup"><span data-stu-id="f8769-109">These settings can be at the tenant-level or at an object level (currently only for groups).</span></span> <span data-ttu-id="f8769-110">Запрос на создание необходимо задать settingValues для всех параметров, определенных в шаблоне.</span><span class="sxs-lookup"><span data-stu-id="f8769-110">The creation request must provide settingValues for all the settings defined in the template.</span></span> <span data-ttu-id="f8769-111">Для определенных параметров может устанавливаться только параметр Управление ли членов группы можно приглашать пользователей гостя.</span><span class="sxs-lookup"><span data-stu-id="f8769-111">For group-specific settings, only the setting governing whether members of a group can invite guest users can be set.</span></span> <span data-ttu-id="f8769-112">Преимущественную это поведение после общедоступной возможность добавления гостевых пользователей в группу.</span><span class="sxs-lookup"><span data-stu-id="f8769-112">This will govern this behavior once the ability to add guest users to a group is generally available.</span></span>

> <span data-ttu-id="f8769-113">**Примечание**: версия /beta этот интерфейс API является только относится к группам.</span><span class="sxs-lookup"><span data-stu-id="f8769-113">**Note**: The /beta version of this API is only applies to groups.</span></span> <span data-ttu-id="f8769-114">Версия /v1.0 этот интерфейс API переименовано в *Создание groupSettings*.</span><span class="sxs-lookup"><span data-stu-id="f8769-114">The /v1.0 version of this API has been renamed to *Create groupSettings*.</span></span>

<span data-ttu-id="f8769-115">Список шаблонов и свойств, которые они поддерживают в бета-версии используйте [directorySettingTemplate запроса](https://developer.microsoft.com/graph/graph-explorer?request=directorySettingTemplates&version=beta).</span><span class="sxs-lookup"><span data-stu-id="f8769-115">For a list of templates and the properties they support in beta, use a [directorySettingTemplate query](https://developer.microsoft.com/graph/graph-explorer?request=directorySettingTemplates&version=beta).</span></span> <span data-ttu-id="f8769-116">(Для конечных точек версии 1.0, вызовите [groupSettingTemplates](https://developer.microsoft.com/graph/graph-explorer?request=groupSettingTemplates&version=v1.0).)</span><span class="sxs-lookup"><span data-stu-id="f8769-116">(For v1.0 endpoints, call [groupSettingTemplates](https://developer.microsoft.com/graph/graph-explorer?request=groupSettingTemplates&version=v1.0).)</span></span>


## <a name="permissions"></a><span data-ttu-id="f8769-117">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f8769-117">Permissions</span></span>
<span data-ttu-id="f8769-p105">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f8769-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f8769-120">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f8769-120">Permission type</span></span>      | <span data-ttu-id="f8769-121">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f8769-121">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f8769-122">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f8769-122">Delegated (work or school account)</span></span> | <span data-ttu-id="f8769-123">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f8769-123">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f8769-124">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f8769-124">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f8769-125">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f8769-125">Not supported.</span></span>    |
|<span data-ttu-id="f8769-126">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f8769-126">Application</span></span> | <span data-ttu-id="f8769-127">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f8769-127">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f8769-128">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f8769-128">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /settings
POST /groups/{id}/settings
```
## <a name="request-headers"></a><span data-ttu-id="f8769-129">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f8769-129">Request headers</span></span>
| <span data-ttu-id="f8769-130">Имя</span><span class="sxs-lookup"><span data-stu-id="f8769-130">Name</span></span>       | <span data-ttu-id="f8769-131">Описание</span><span class="sxs-lookup"><span data-stu-id="f8769-131">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="f8769-132">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f8769-132">Authorization</span></span>  | <span data-ttu-id="f8769-p106">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f8769-p106">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f8769-135">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f8769-135">Request body</span></span>
<span data-ttu-id="f8769-136">В тексте запроса укажите представление JSON объекта [directorySetting](../resources/directorysetting.md) .</span><span class="sxs-lookup"><span data-stu-id="f8769-136">In the request body, supply a JSON representation of [directorySetting](../resources/directorysetting.md) object.</span></span>  <span data-ttu-id="f8769-137">Тем не менее отображаемое имя для параметра задается в соответствии на имя шаблона параметров, который указывает ссылка.</span><span class="sxs-lookup"><span data-stu-id="f8769-137">However, the display name for the setting will be set based on the referenced settings template name.</span></span>

## <a name="response"></a><span data-ttu-id="f8769-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="f8769-138">Response</span></span>

<span data-ttu-id="f8769-139">Успешно завершена, этот метод возвращает `201 Created` объект [directorySetting](../resources/directorysetting.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="f8769-139">If successful, this method returns `201 Created` response code and [directorySetting](../resources/directorysetting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f8769-140">Пример</span><span class="sxs-lookup"><span data-stu-id="f8769-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f8769-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="f8769-141">Request</span></span>
<span data-ttu-id="f8769-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f8769-142">Here is an example of the request.</span></span>
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
<span data-ttu-id="f8769-143">В тексте запроса укажите представление JSON объекта [directorySetting](../resources/directorysetting.md) .</span><span class="sxs-lookup"><span data-stu-id="f8769-143">In the request body, supply a JSON representation of [directorySetting](../resources/directorysetting.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="f8769-144">Ответ</span><span class="sxs-lookup"><span data-stu-id="f8769-144">Response</span></span>
<span data-ttu-id="f8769-p108">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="f8769-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "Error: /api-reference/beta/api/directorysetting-post-settings.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
