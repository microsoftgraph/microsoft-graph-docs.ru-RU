---
title: Тип enum deviceManagementConfigurationControlType
description: Представление типа управления "Настройка" в UX
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 183496c68f836f04adadacecb80fab066f619def
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50162495"
---
# <a name="devicemanagementconfigurationcontroltype-enum-type"></a><span data-ttu-id="77de2-103">Тип enum deviceManagementConfigurationControlType</span><span class="sxs-lookup"><span data-stu-id="77de2-103">deviceManagementConfigurationControlType enum type</span></span>

<span data-ttu-id="77de2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="77de2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="77de2-105">**Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="77de2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="77de2-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="77de2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="77de2-107">Представление типа управления "Настройка" в UX</span><span class="sxs-lookup"><span data-stu-id="77de2-107">Setting control type representation in the UX</span></span>

## <a name="members"></a><span data-ttu-id="77de2-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="77de2-108">Members</span></span>
|<span data-ttu-id="77de2-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="77de2-109">Member</span></span>|<span data-ttu-id="77de2-110">Значение</span><span class="sxs-lookup"><span data-stu-id="77de2-110">Value</span></span>|<span data-ttu-id="77de2-111">Описание</span><span class="sxs-lookup"><span data-stu-id="77de2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="77de2-112">default</span><span class="sxs-lookup"><span data-stu-id="77de2-112">default</span></span>|<span data-ttu-id="77de2-113">0</span><span class="sxs-lookup"><span data-stu-id="77de2-113">0</span></span>|<span data-ttu-id="77de2-114">Не переопределяйте значение по умолчанию</span><span class="sxs-lookup"><span data-stu-id="77de2-114">Don’t override default</span></span>|
|<span data-ttu-id="77de2-115">dropdown</span><span class="sxs-lookup"><span data-stu-id="77de2-115">dropdown</span></span>|<span data-ttu-id="77de2-116">1 </span><span class="sxs-lookup"><span data-stu-id="77de2-116">1</span></span>|<span data-ttu-id="77de2-117">Выбор отображения в выпадаемом окном</span><span class="sxs-lookup"><span data-stu-id="77de2-117">Display Choice in dropdown</span></span>|
|<span data-ttu-id="77de2-118">smallTextBox</span><span class="sxs-lookup"><span data-stu-id="77de2-118">smallTextBox</span></span>|<span data-ttu-id="77de2-119">2 </span><span class="sxs-lookup"><span data-stu-id="77de2-119">2</span></span>|<span data-ttu-id="77de2-120">Отображение ввода текста в небольших текстовых вводимых данных</span><span class="sxs-lookup"><span data-stu-id="77de2-120">Display text input in small text input</span></span>|
|<span data-ttu-id="77de2-121">largeTextBox</span><span class="sxs-lookup"><span data-stu-id="77de2-121">largeTextBox</span></span>|<span data-ttu-id="77de2-122">3 </span><span class="sxs-lookup"><span data-stu-id="77de2-122">3</span></span>|<span data-ttu-id="77de2-123">Отображение ввода текста при большом текстовом вводе</span><span class="sxs-lookup"><span data-stu-id="77de2-123">Display text input in large text input</span></span>|
|<span data-ttu-id="77de2-124">toggle</span><span class="sxs-lookup"><span data-stu-id="77de2-124">toggle</span></span>|<span data-ttu-id="77de2-125">4 </span><span class="sxs-lookup"><span data-stu-id="77de2-125">4</span></span>|<span data-ttu-id="77de2-126">Разрешить тип управления "Перегной"</span><span class="sxs-lookup"><span data-stu-id="77de2-126">Allow for toggle control type</span></span>|
|<span data-ttu-id="77de2-127">multiheaderGrid</span><span class="sxs-lookup"><span data-stu-id="77de2-127">multiheaderGrid</span></span>|<span data-ttu-id="77de2-128">5 </span><span class="sxs-lookup"><span data-stu-id="77de2-128">5</span></span>|<span data-ttu-id="77de2-129">Разрешить тип многозаголовой сетки</span><span class="sxs-lookup"><span data-stu-id="77de2-129">Allow for multiheader grid control type</span></span>|
|<span data-ttu-id="77de2-130">contextPane</span><span class="sxs-lookup"><span data-stu-id="77de2-130">contextPane</span></span>|<span data-ttu-id="77de2-131">6 </span><span class="sxs-lookup"><span data-stu-id="77de2-131">6</span></span>|<span data-ttu-id="77de2-132">Разрешить тип управления области контекста</span><span class="sxs-lookup"><span data-stu-id="77de2-132">Allow for context pane control type</span></span>|




