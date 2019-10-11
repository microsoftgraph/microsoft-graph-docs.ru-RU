---
title: Обновление фотографии команды
description: Вы можете обновить фотографию (изображение) для команды.
author: clearab
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 6c19e09713d16f8c2739b1a8398509953a19ddd0
ms.sourcegitcommit: f23cc661a0e30d01a6b59cfdae90768c55b80ae2
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/08/2019
ms.locfileid: "37418337"
---
# <a name="update-team-photo"></a><span data-ttu-id="d2d11-103">Обновление фотографии команды</span><span class="sxs-lookup"><span data-stu-id="d2d11-103">Update team photo</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d2d11-104">Вы можете обновить фотографию (изображение) для команды.</span><span class="sxs-lookup"><span data-stu-id="d2d11-104">Update the photo (picture) for a team.</span></span> <span data-ttu-id="d2d11-105">Поддерживаемые размеры фотографий в формате HD для Office 365: 48 x 48, 64 x 64, 96 x 96, 120 x 120, 240 x 240, 360 x 360, 432 x 432, 504 x 504 и 648 x 648.</span><span class="sxs-lookup"><span data-stu-id="d2d11-105">The supported sizes of HD photos in Office 365 are as follows: 48x48, 64x64, 96x96, 120x120, 240x240, 360x360, 432x432, 504x504, and 648x648.</span></span> <span data-ttu-id="d2d11-106">Фотографии, хранящиеся в Azure Active Directory, могут быть любого размера.</span><span class="sxs-lookup"><span data-stu-id="d2d11-106">Photos can be any dimension if they are stored in Azure Active Directory.</span></span>

> [!Note]
> <span data-ttu-id="d2d11-107">Общий размер запроса не должен превышать 4 МБ.</span><span class="sxs-lookup"><span data-stu-id="d2d11-107">There is a limit of 4 MB on the total size of the request.</span></span> <span data-ttu-id="d2d11-108">Таким образом, размер фотографии составит менее 4 МБ.</span><span class="sxs-lookup"><span data-stu-id="d2d11-108">This limits the photo size to less than 4 MB.</span></span>

## <a name="permissions"></a><span data-ttu-id="d2d11-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d2d11-109">Permissions</span></span>

<span data-ttu-id="d2d11-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d2d11-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d2d11-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d2d11-112">Permission type</span></span>      | <span data-ttu-id="d2d11-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d2d11-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d2d11-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d2d11-114">Delegated (work or school account)</span></span> | <span data-ttu-id="d2d11-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d2d11-115">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="d2d11-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d2d11-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d2d11-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d2d11-117">Not supported.</span></span>    |
|<span data-ttu-id="d2d11-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d2d11-118">Application</span></span> | <span data-ttu-id="d2d11-119">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d2d11-119">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d2d11-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d2d11-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}-->

```http
PUT /beta/teams/{id}/photo
```

## <a name="request-headers"></a><span data-ttu-id="d2d11-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d2d11-121">Request headers</span></span>

| <span data-ttu-id="d2d11-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d2d11-122">Header</span></span>        | <span data-ttu-id="d2d11-123">Значение</span><span class="sxs-lookup"><span data-stu-id="d2d11-123">Value</span></span>           |
|:--------------|:--------------  |
| <span data-ttu-id="d2d11-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d2d11-124">Authorization</span></span> | <span data-ttu-id="d2d11-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d2d11-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="d2d11-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d2d11-127">Content-type</span></span> | <span data-ttu-id="d2d11-p105">image/jpeg. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d2d11-p105">image/jpeg. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d2d11-130">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d2d11-130">Request body</span></span>

<span data-ttu-id="d2d11-131">В текст запроса нужно включить двоичные данные фотографии.</span><span class="sxs-lookup"><span data-stu-id="d2d11-131">In the request body, include the binary data of the photo in the request body.</span></span>

## <a name="response"></a><span data-ttu-id="d2d11-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="d2d11-132">Response</span></span>

<span data-ttu-id="d2d11-133">В случае успешного выполнения этот метод возвращает код отклика `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="d2d11-133">If successful, this method returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="d2d11-134">Пример</span><span class="sxs-lookup"><span data-stu-id="d2d11-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="d2d11-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="d2d11-135">Request</span></span>

<span data-ttu-id="d2d11-136">Ниже приведен пример запроса на обновление фотографии команды.</span><span class="sxs-lookup"><span data-stu-id="d2d11-136">Here is an example of the request to update a team photo.</span></span>

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

### <a name="response"></a><span data-ttu-id="d2d11-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="d2d11-137">Response</span></span> 

<span data-ttu-id="d2d11-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d2d11-138">Here is an example of the response.</span></span>

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
