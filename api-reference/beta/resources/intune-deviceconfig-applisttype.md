---
title: Тип перечисления appListType
description: Возможные значения список соответствия требованиям приложения.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: eb2b4afa6639d70b81a59bda1250ea9ed231ccdb
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27939646"
---
# <a name="applisttype-enum-type"></a><span data-ttu-id="29ef9-103">Тип перечисления appListType</span><span class="sxs-lookup"><span data-stu-id="29ef9-103">appListType enum type</span></span>

> <span data-ttu-id="29ef9-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="29ef9-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="29ef9-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="29ef9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="29ef9-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="29ef9-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="29ef9-107">Возможные значения список соответствия требованиям приложения.</span><span class="sxs-lookup"><span data-stu-id="29ef9-107">Possible values of the compliance app list.</span></span>
## <a name="members"></a><span data-ttu-id="29ef9-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="29ef9-108">Members</span></span>
|<span data-ttu-id="29ef9-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="29ef9-109">Member</span></span>|<span data-ttu-id="29ef9-110">Значение</span><span class="sxs-lookup"><span data-stu-id="29ef9-110">Value</span></span>|<span data-ttu-id="29ef9-111">Описание</span><span class="sxs-lookup"><span data-stu-id="29ef9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="29ef9-112">Нет</span><span class="sxs-lookup"><span data-stu-id="29ef9-112">none</span></span>|<span data-ttu-id="29ef9-113">0</span><span class="sxs-lookup"><span data-stu-id="29ef9-113">0</span></span>|<span data-ttu-id="29ef9-114">Значение по умолчанию, без цели.</span><span class="sxs-lookup"><span data-stu-id="29ef9-114">Default value, no intent.</span></span>|
|<span data-ttu-id="29ef9-115">appsInListCompliant</span><span class="sxs-lookup"><span data-stu-id="29ef9-115">appsInListCompliant</span></span>|<span data-ttu-id="29ef9-116">1</span><span class="sxs-lookup"><span data-stu-id="29ef9-116">1</span></span>|<span data-ttu-id="29ef9-117">Список представляет приложений, которые будут считаться спецификации (только для приложений в списке совместимых).</span><span class="sxs-lookup"><span data-stu-id="29ef9-117">The list represents the apps that will be considered compliant (only apps on the list are compliant).</span></span>|
|<span data-ttu-id="29ef9-118">appsNotInListCompliant</span><span class="sxs-lookup"><span data-stu-id="29ef9-118">appsNotInListCompliant</span></span>|<span data-ttu-id="29ef9-119">2</span><span class="sxs-lookup"><span data-stu-id="29ef9-119">2</span></span>|<span data-ttu-id="29ef9-120">Представляет список приложений, которые будут считаться несовместимой (все приложения совместимых за исключением приложений в списке).</span><span class="sxs-lookup"><span data-stu-id="29ef9-120">The list represents the apps that will be considered non compliant (all apps are compliant except apps on the list).</span></span>|





