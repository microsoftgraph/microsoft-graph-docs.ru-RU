---
title: Тип ресурса АадусернотификатионреЦипиент
description: Представляет получателя Azure Active Directory (Azure AD) для уведомления, отправленного в веб-канале активности Microsoft Teams.
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 118951336a031548a557f94df8b2b2068e415408
ms.sourcegitcommit: 6201b3a5646f640f25a68ab033eca9eb60ccd05e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/21/2020
ms.locfileid: "49377570"
---
# <a name="aadusernotificationrecipient-resource-type"></a><span data-ttu-id="d2fbf-103">Тип ресурса АадусернотификатионреЦипиент</span><span class="sxs-lookup"><span data-stu-id="d2fbf-103">aadUserNotificationRecipient resource type</span></span>

<span data-ttu-id="d2fbf-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d2fbf-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d2fbf-105">Представляет получателя Azure Active Directory (Azure AD) для уведомления, отправленного в веб-канале активности Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="d2fbf-105">Represents an Azure Active Directory (Azure AD) user recipient of a notification sent in a Microsoft Teams activity feed.</span></span>

<span data-ttu-id="d2fbf-106">Наследуется от [теамворкнотификатионреЦипиент](teamworknotificationrecipient.md).</span><span class="sxs-lookup"><span data-stu-id="d2fbf-106">Inherits from [teamworkNotificationRecipient](teamworknotificationrecipient.md).</span></span>

## <a name="properties"></a><span data-ttu-id="d2fbf-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="d2fbf-107">Properties</span></span>
|<span data-ttu-id="d2fbf-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="d2fbf-108">Property</span></span>|<span data-ttu-id="d2fbf-109">Тип</span><span class="sxs-lookup"><span data-stu-id="d2fbf-109">Type</span></span>|<span data-ttu-id="d2fbf-110">Описание</span><span class="sxs-lookup"><span data-stu-id="d2fbf-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d2fbf-111">userId</span><span class="sxs-lookup"><span data-stu-id="d2fbf-111">userId</span></span>|<span data-ttu-id="d2fbf-112">String</span><span class="sxs-lookup"><span data-stu-id="d2fbf-112">String</span></span>|<span data-ttu-id="d2fbf-113">Идентификатор пользователя Azure AD.</span><span class="sxs-lookup"><span data-stu-id="d2fbf-113">Azure AD user identifier.</span></span> <span data-ttu-id="d2fbf-114">Для получения этого идентификатора используйте метод [List Users](../api/user-list.md) .</span><span class="sxs-lookup"><span data-stu-id="d2fbf-114">Use the [List users](../api/user-list.md) method to get this ID.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d2fbf-115">Связи</span><span class="sxs-lookup"><span data-stu-id="d2fbf-115">Relationships</span></span>
<span data-ttu-id="d2fbf-116">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="d2fbf-116">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d2fbf-117">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="d2fbf-117">JSON representation</span></span>
<span data-ttu-id="d2fbf-118">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d2fbf-118">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.aadUserNotificationRecipient"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.aadUserNotificationRecipient",
  "userId": "String"
}
```

