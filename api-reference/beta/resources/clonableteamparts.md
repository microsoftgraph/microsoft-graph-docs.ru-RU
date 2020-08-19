---
title: тип перечисления Клонаблетеампартс
description: 'Описывает, какая часть команды должна быть клонирована. '
localization_priority: Normal
doc_type: enumPageType
ms.prod: ''
author: nkramer
ms.openlocfilehash: e08beeb232e5c9b2c77200f75053e3a822945ca6
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46810589"
---
# <a name="clonableteamparts-enum-type"></a><span data-ttu-id="e0ee0-103">тип перечисления Клонаблетеампартс</span><span class="sxs-lookup"><span data-stu-id="e0ee0-103">clonableTeamParts enum type</span></span>

<span data-ttu-id="e0ee0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e0ee0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e0ee0-105">Описывает, какая часть [команды](../resources/team.md) должна быть клонирована.</span><span class="sxs-lookup"><span data-stu-id="e0ee0-105">Describes which part of a [team](../resources/team.md) should be cloned.</span></span>

## <a name="members"></a><span data-ttu-id="e0ee0-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="e0ee0-106">Members</span></span>

| <span data-ttu-id="e0ee0-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="e0ee0-107">Member</span></span> | <span data-ttu-id="e0ee0-108">Значение</span><span class="sxs-lookup"><span data-stu-id="e0ee0-108">Value</span></span>| <span data-ttu-id="e0ee0-109">Описание</span><span class="sxs-lookup"><span data-stu-id="e0ee0-109">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="e0ee0-110">apps</span><span class="sxs-lookup"><span data-stu-id="e0ee0-110">apps</span></span>|<span data-ttu-id="e0ee0-111">1,1</span><span class="sxs-lookup"><span data-stu-id="e0ee0-111">1</span></span>|<span data-ttu-id="e0ee0-112">Скопируйте список установленных приложений.</span><span class="sxs-lookup"><span data-stu-id="e0ee0-112">Copy the list of installed apps.</span></span>|
|<span data-ttu-id="e0ee0-113">tabs</span><span class="sxs-lookup"><span data-stu-id="e0ee0-113">tabs</span></span>|<span data-ttu-id="e0ee0-114">2</span><span class="sxs-lookup"><span data-stu-id="e0ee0-114">2</span></span>|<span data-ttu-id="e0ee0-115">копирует вкладки в каналах.</span><span class="sxs-lookup"><span data-stu-id="e0ee0-115">copies the tabs within channels.</span></span>|
|<span data-ttu-id="e0ee0-116">settings</span><span class="sxs-lookup"><span data-stu-id="e0ee0-116">settings</span></span>|<span data-ttu-id="e0ee0-117">4 </span><span class="sxs-lookup"><span data-stu-id="e0ee0-117">4</span></span>|<span data-ttu-id="e0ee0-118">Копирует все параметры в группе вместе с параметрами группы ключей.</span><span class="sxs-lookup"><span data-stu-id="e0ee0-118">Copies all settings within the team, along with key group settings.</span></span>|
|<span data-ttu-id="e0ee0-119">channels</span><span class="sxs-lookup"><span data-stu-id="e0ee0-119">channels</span></span>|<span data-ttu-id="e0ee0-120">8 </span><span class="sxs-lookup"><span data-stu-id="e0ee0-120">8</span></span>|<span data-ttu-id="e0ee0-121">копирует структуру канала (но не сообщения в канале).</span><span class="sxs-lookup"><span data-stu-id="e0ee0-121">copies the channel structure (but not the messages in the channel).</span></span>|
|<span data-ttu-id="e0ee0-122">members</span><span class="sxs-lookup"><span data-stu-id="e0ee0-122">members</span></span>|<span data-ttu-id="e0ee0-123">16 </span><span class="sxs-lookup"><span data-stu-id="e0ee0-123">16</span></span>|<span data-ttu-id="e0ee0-124">копирует участников и владельцев группы.</span><span class="sxs-lookup"><span data-stu-id="e0ee0-124">copies the members and owners of the team.</span></span>|
