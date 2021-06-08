---
title: тип ресурса aadUserNotificationRecipient
description: Представляет получателя Azure Active Directory пользователя Azure AD, отправимого в канале Microsoft Teams действий.
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: ec8e05a09af27ca6092da24e13a604fdd7e013f4
ms.sourcegitcommit: a2d81138de2a0404e611fbb535679199477ef3d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/08/2021
ms.locfileid: "52813201"
---
# <a name="aadusernotificationrecipient-resource-type"></a><span data-ttu-id="17557-103">тип ресурса aadUserNotificationRecipient</span><span class="sxs-lookup"><span data-stu-id="17557-103">aadUserNotificationRecipient resource type</span></span>

<span data-ttu-id="17557-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="17557-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="17557-105">Представляет получателя Azure Active Directory пользователя Azure AD, отправимого в канале Microsoft Teams действий.</span><span class="sxs-lookup"><span data-stu-id="17557-105">Represents an Azure Active Directory (Azure AD) user recipient of a notification sent in a Microsoft Teams activity feed.</span></span>

<span data-ttu-id="17557-106">Наследует [от teamworkNotificationRecipient](teamworknotificationrecipient.md).</span><span class="sxs-lookup"><span data-stu-id="17557-106">Inherits from [teamworkNotificationRecipient](teamworknotificationrecipient.md).</span></span>

## <a name="properties"></a><span data-ttu-id="17557-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="17557-107">Properties</span></span>
|<span data-ttu-id="17557-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="17557-108">Property</span></span>|<span data-ttu-id="17557-109">Тип</span><span class="sxs-lookup"><span data-stu-id="17557-109">Type</span></span>|<span data-ttu-id="17557-110">Описание</span><span class="sxs-lookup"><span data-stu-id="17557-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="17557-111">userId</span><span class="sxs-lookup"><span data-stu-id="17557-111">userId</span></span>|<span data-ttu-id="17557-112">String</span><span class="sxs-lookup"><span data-stu-id="17557-112">String</span></span>|<span data-ttu-id="17557-113">Идентификатор пользователя Azure AD.</span><span class="sxs-lookup"><span data-stu-id="17557-113">Azure AD user identifier.</span></span> <span data-ttu-id="17557-114">Чтобы получить [этот](../api/user-list.md) ID, используйте метод пользователей списка.</span><span class="sxs-lookup"><span data-stu-id="17557-114">Use the [List users](../api/user-list.md) method to get this ID.</span></span>|

## <a name="relationships"></a><span data-ttu-id="17557-115">Связи</span><span class="sxs-lookup"><span data-stu-id="17557-115">Relationships</span></span>
<span data-ttu-id="17557-116">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="17557-116">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="17557-117">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="17557-117">JSON representation</span></span>
<span data-ttu-id="17557-118">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="17557-118">The following is a JSON representation of the resource.</span></span>
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

