---
title: Тип перечисления appListType
description: Возможные значения список соответствия требованиям приложения.
ms.openlocfilehash: 3fcfecde8dbc9efe92f842e9d2b45b7f1579c217
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27079839"
---
# <a name="applisttype-enum-type"></a><span data-ttu-id="9a9ff-103">Тип перечисления appListType</span><span class="sxs-lookup"><span data-stu-id="9a9ff-103">appListType enum type</span></span>

> <span data-ttu-id="9a9ff-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="9a9ff-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9a9ff-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9a9ff-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9a9ff-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="9a9ff-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9a9ff-107">Возможные значения список соответствия требованиям приложения.</span><span class="sxs-lookup"><span data-stu-id="9a9ff-107">Possible values of the compliance app list.</span></span>
## <a name="members"></a><span data-ttu-id="9a9ff-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="9a9ff-108">Members</span></span>
|<span data-ttu-id="9a9ff-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="9a9ff-109">Member</span></span>|<span data-ttu-id="9a9ff-110">Значение</span><span class="sxs-lookup"><span data-stu-id="9a9ff-110">Value</span></span>|<span data-ttu-id="9a9ff-111">Description</span><span class="sxs-lookup"><span data-stu-id="9a9ff-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9a9ff-112">Нет</span><span class="sxs-lookup"><span data-stu-id="9a9ff-112">none</span></span>|<span data-ttu-id="9a9ff-113">0</span><span class="sxs-lookup"><span data-stu-id="9a9ff-113">0</span></span>|<span data-ttu-id="9a9ff-114">Значение по умолчанию, без цели.</span><span class="sxs-lookup"><span data-stu-id="9a9ff-114">Default value, no intent.</span></span>|
|<span data-ttu-id="9a9ff-115">appsInListCompliant</span><span class="sxs-lookup"><span data-stu-id="9a9ff-115">appsInListCompliant</span></span>|<span data-ttu-id="9a9ff-116">1</span><span class="sxs-lookup"><span data-stu-id="9a9ff-116">1</span></span>|<span data-ttu-id="9a9ff-117">Список представляет приложений, которые будут считаться спецификации (только для приложений в списке совместимых).</span><span class="sxs-lookup"><span data-stu-id="9a9ff-117">The list represents the apps that will be considered compliant (only apps on the list are compliant).</span></span>|
|<span data-ttu-id="9a9ff-118">appsNotInListCompliant</span><span class="sxs-lookup"><span data-stu-id="9a9ff-118">appsNotInListCompliant</span></span>|<span data-ttu-id="9a9ff-119">2</span><span class="sxs-lookup"><span data-stu-id="9a9ff-119">2</span></span>|<span data-ttu-id="9a9ff-120">Представляет список приложений, которые будут считаться несовместимой (все приложения совместимых за исключением приложений в списке).</span><span class="sxs-lookup"><span data-stu-id="9a9ff-120">The list represents the apps that will be considered non compliant (all apps are compliant except apps on the list).</span></span>|





