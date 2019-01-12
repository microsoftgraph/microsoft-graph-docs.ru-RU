---
title: Тип перечисления firewallPreSharedKeyEncodingMethodType
description: Возможные значения для firewallPreSharedKeyEncodingMethod
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 513a6c545fedc73add4e710ed784ef223d1f8539
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27976354"
---
# <a name="firewallpresharedkeyencodingmethodtype-enum-type"></a><span data-ttu-id="55ca0-103">Тип перечисления firewallPreSharedKeyEncodingMethodType</span><span class="sxs-lookup"><span data-stu-id="55ca0-103">firewallPreSharedKeyEncodingMethodType enum type</span></span>

> <span data-ttu-id="55ca0-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="55ca0-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="55ca0-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="55ca0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="55ca0-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="55ca0-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="55ca0-107">Возможные значения для firewallPreSharedKeyEncodingMethod</span><span class="sxs-lookup"><span data-stu-id="55ca0-107">Possible values for firewallPreSharedKeyEncodingMethod</span></span>
## <a name="members"></a><span data-ttu-id="55ca0-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="55ca0-108">Members</span></span>
|<span data-ttu-id="55ca0-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="55ca0-109">Member</span></span>|<span data-ttu-id="55ca0-110">Значение</span><span class="sxs-lookup"><span data-stu-id="55ca0-110">Value</span></span>|<span data-ttu-id="55ca0-111">Описание</span><span class="sxs-lookup"><span data-stu-id="55ca0-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="55ca0-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="55ca0-112">deviceDefault</span></span>|<span data-ttu-id="55ca0-113">0</span><span class="sxs-lookup"><span data-stu-id="55ca0-113">0</span></span>|<span data-ttu-id="55ca0-114">Значение не настраивается с Intune, не переопределяют настраиваемых пользователем устройства по умолчанию</span><span class="sxs-lookup"><span data-stu-id="55ca0-114">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="55ca0-115">Нет</span><span class="sxs-lookup"><span data-stu-id="55ca0-115">none</span></span>|<span data-ttu-id="55ca0-116">1</span><span class="sxs-lookup"><span data-stu-id="55ca0-116">1</span></span>|<span data-ttu-id="55ca0-117">Предварительный ключ не кодируются.</span><span class="sxs-lookup"><span data-stu-id="55ca0-117">Preshared key is not encoded.</span></span> <span data-ttu-id="55ca0-118">Вместо этого он будет храниться в формате Юникода</span><span class="sxs-lookup"><span data-stu-id="55ca0-118">Instead, it is kept in its wide-character format</span></span>|
|<span data-ttu-id="55ca0-119">utF8</span><span class="sxs-lookup"><span data-stu-id="55ca0-119">utF8</span></span>|<span data-ttu-id="55ca0-120">2</span><span class="sxs-lookup"><span data-stu-id="55ca0-120">2</span></span>|<span data-ttu-id="55ca0-121">Кодирование предварительный ключ, используя UTF-8</span><span class="sxs-lookup"><span data-stu-id="55ca0-121">Encode the preshared key using UTF-8</span></span>|





