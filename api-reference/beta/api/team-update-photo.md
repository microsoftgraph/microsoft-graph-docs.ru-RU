---
title: Обновление фотографии команды
description: Вы можете обновить фотографию (изображение) для команды.
author: clearab
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 22fdca19b657bdf439f356fb61e4f805f45b4f4b
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/26/2020
ms.locfileid: "44896128"
---
# <a name="update-team-photo"></a><span data-ttu-id="a7f78-103">Обновление фотографии команды</span><span class="sxs-lookup"><span data-stu-id="a7f78-103">Update team photo</span></span>

<span data-ttu-id="a7f78-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a7f78-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a7f78-105">Вы можете обновить фотографию (изображение) для команды.</span><span class="sxs-lookup"><span data-stu-id="a7f78-105">Update the photo (picture) for a team.</span></span> <span data-ttu-id="a7f78-106">Ниже приведены поддерживаемые размеры фотографий HD в Microsoft 365:48x48, 64x64, 96x96, 120x120, 240x240, 360 x 360, 432 x 432, 504 504 и 648x648 Пиксели.</span><span class="sxs-lookup"><span data-stu-id="a7f78-106">The following are the supported sizes of HD photos in Microsoft 365: 48x48, 64x64, 96x96, 120x120, 240x240, 360x360, 432x432, 504x504, and 648x648 pixels.</span></span> <span data-ttu-id="a7f78-107">Фотографии, хранящиеся в Azure Active Directory, могут быть любого размера.</span><span class="sxs-lookup"><span data-stu-id="a7f78-107">Photos can be any dimension if they are stored in Azure Active Directory.</span></span>

> [!Note]
> <span data-ttu-id="a7f78-108">Общий размер запроса не должен превышать 4 МБ.</span><span class="sxs-lookup"><span data-stu-id="a7f78-108">There is a limit of 4 MB on the total size of the request.</span></span> <span data-ttu-id="a7f78-109">Таким образом, размер фотографии составит менее 4 МБ.</span><span class="sxs-lookup"><span data-stu-id="a7f78-109">This limits the photo size to less than 4 MB.</span></span>

## <a name="permissions"></a><span data-ttu-id="a7f78-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a7f78-110">Permissions</span></span>

<span data-ttu-id="a7f78-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a7f78-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a7f78-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a7f78-113">Permission type</span></span>      | <span data-ttu-id="a7f78-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a7f78-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a7f78-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a7f78-115">Delegated (work or school account)</span></span> | <span data-ttu-id="a7f78-116">Теамсеттингс. ReadWrite. ALL, Group. ReadWrite. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="a7f78-116">TeamSettings.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="a7f78-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a7f78-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a7f78-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a7f78-118">Not supported.</span></span>    |
|<span data-ttu-id="a7f78-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a7f78-119">Application</span></span> | <span data-ttu-id="a7f78-120">Теамсеттингс. Edit. Group \*, Теамсеттингс. ReadWrite. ALL, Group. ReadWrite. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="a7f78-120">TeamSettings.Edit.Group\*, TeamSettings.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="a7f78-121">**Note**: разрешения, помеченные как \* использовать [согласие с определенным ресурсом](https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="a7f78-121">**Note**: Permissions marked with \* use [resource-specific consent](https://aka.ms/teams-rsc).</span></span>

> <span data-ttu-id="a7f78-122">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="a7f78-122">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="a7f78-123">Глобальные администраторы и администраторы службы Microsoft Teams могут получать доступ к командам, в которых они не состоят.</span><span class="sxs-lookup"><span data-stu-id="a7f78-123">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="a7f78-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a7f78-124">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}-->

```http
PUT /teams/{id}/photo
```

## <a name="request-headers"></a><span data-ttu-id="a7f78-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a7f78-125">Request headers</span></span>

| <span data-ttu-id="a7f78-126">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a7f78-126">Header</span></span>        | <span data-ttu-id="a7f78-127">Значение</span><span class="sxs-lookup"><span data-stu-id="a7f78-127">Value</span></span>           |
|:--------------|:--------------  |
| <span data-ttu-id="a7f78-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a7f78-128">Authorization</span></span> | <span data-ttu-id="a7f78-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a7f78-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="a7f78-131">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a7f78-131">Content-type</span></span> | <span data-ttu-id="a7f78-p106">image/jpeg. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a7f78-p106">image/jpeg. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a7f78-134">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a7f78-134">Request body</span></span>

<span data-ttu-id="a7f78-135">В текст запроса нужно включить двоичные данные фотографии.</span><span class="sxs-lookup"><span data-stu-id="a7f78-135">In the request body, include the binary data of the photo.</span></span>

## <a name="response"></a><span data-ttu-id="a7f78-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="a7f78-136">Response</span></span>

<span data-ttu-id="a7f78-137">В случае успешного выполнения этот метод возвращает код отклика `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="a7f78-137">If successful, this method returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="a7f78-138">Пример</span><span class="sxs-lookup"><span data-stu-id="a7f78-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="a7f78-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="a7f78-139">Request</span></span>

<span data-ttu-id="a7f78-140">Ниже приведен пример запроса на обновление фотографии команды.</span><span class="sxs-lookup"><span data-stu-id="a7f78-140">Here is an example of the request to update a team photo.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "update_team_photo"
}-->
```http
PUT https://graph.microsoft.com/beta/teams/{id}/photo
Content-type: image/jpeg

{
  <Binary data for the image>
}
```

### <a name="response"></a><span data-ttu-id="a7f78-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="a7f78-141">Response</span></span> 

<span data-ttu-id="a7f78-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a7f78-142">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update team photo",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
