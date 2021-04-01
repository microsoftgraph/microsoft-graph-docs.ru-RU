---
title: тип ресурса aadUserNotificationRecipient
description: Представляет получателя пользователя Azure Active Directory (Azure AD) с уведомлением, отправленным в канале действий Microsoft Teams.
author: eddie-lee-msft
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: dadb08dad99f6c4fd6857e8e60f457ea51811de1
ms.sourcegitcommit: 17f1c9cff2e59049b894db32435af02e4ae32a70
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "51474147"
---
# <a name="aadusernotificationrecipient-resource-type"></a><span data-ttu-id="da24e-103">тип ресурса aadUserNotificationRecipient</span><span class="sxs-lookup"><span data-stu-id="da24e-103">aadUserNotificationRecipient resource type</span></span>

<span data-ttu-id="da24e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="da24e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="da24e-105">Представляет получателя пользователя Azure Active Directory (Azure AD) с уведомлением, отправленным в канале действий Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="da24e-105">Represents an Azure Active Directory (Azure AD) user recipient of a notification sent in a Microsoft Teams activity feed.</span></span>

<span data-ttu-id="da24e-106">Наследует [от teamworkNotificationRecipient](teamworknotificationrecipient.md).</span><span class="sxs-lookup"><span data-stu-id="da24e-106">Inherits from [teamworkNotificationRecipient](teamworknotificationrecipient.md).</span></span>

## <a name="properties"></a><span data-ttu-id="da24e-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="da24e-107">Properties</span></span>
|<span data-ttu-id="da24e-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="da24e-108">Property</span></span>|<span data-ttu-id="da24e-109">Тип</span><span class="sxs-lookup"><span data-stu-id="da24e-109">Type</span></span>|<span data-ttu-id="da24e-110">Описание</span><span class="sxs-lookup"><span data-stu-id="da24e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="da24e-111">userId</span><span class="sxs-lookup"><span data-stu-id="da24e-111">userId</span></span>|<span data-ttu-id="da24e-112">String</span><span class="sxs-lookup"><span data-stu-id="da24e-112">String</span></span>|<span data-ttu-id="da24e-113">Идентификатор пользователя Azure AD.</span><span class="sxs-lookup"><span data-stu-id="da24e-113">Azure AD user identifier.</span></span> <span data-ttu-id="da24e-114">Чтобы получить [этот](../api/user-list.md) ID, используйте метод пользователей списка.</span><span class="sxs-lookup"><span data-stu-id="da24e-114">Use the [List users](../api/user-list.md) method to get this ID.</span></span>|

## <a name="relationships"></a><span data-ttu-id="da24e-115">Связи</span><span class="sxs-lookup"><span data-stu-id="da24e-115">Relationships</span></span>
<span data-ttu-id="da24e-116">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="da24e-116">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="da24e-117">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="da24e-117">JSON representation</span></span>
<span data-ttu-id="da24e-118">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="da24e-118">The following is a JSON representation of the resource.</span></span>
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

