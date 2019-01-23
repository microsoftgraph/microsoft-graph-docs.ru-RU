---
title: Тип перечисления firewallPreSharedKeyEncodingMethodType
description: Возможные значения для firewallPreSharedKeyEncodingMethod
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 577925f141c6dd94b493664d3617df939d19c5c6
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29410954"
---
# <a name="firewallpresharedkeyencodingmethodtype-enum-type"></a><span data-ttu-id="b7e78-103">Тип перечисления firewallPreSharedKeyEncodingMethodType</span><span class="sxs-lookup"><span data-stu-id="b7e78-103">firewallPreSharedKeyEncodingMethodType enum type</span></span>

> <span data-ttu-id="b7e78-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="b7e78-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="b7e78-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b7e78-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b7e78-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b7e78-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b7e78-107">Возможные значения для firewallPreSharedKeyEncodingMethod</span><span class="sxs-lookup"><span data-stu-id="b7e78-107">Possible values for firewallPreSharedKeyEncodingMethod</span></span>

## <a name="members"></a><span data-ttu-id="b7e78-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="b7e78-108">Members</span></span>
|<span data-ttu-id="b7e78-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="b7e78-109">Member</span></span>|<span data-ttu-id="b7e78-110">Значение</span><span class="sxs-lookup"><span data-stu-id="b7e78-110">Value</span></span>|<span data-ttu-id="b7e78-111">Описание</span><span class="sxs-lookup"><span data-stu-id="b7e78-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b7e78-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="b7e78-112">deviceDefault</span></span>|<span data-ttu-id="b7e78-113">0</span><span class="sxs-lookup"><span data-stu-id="b7e78-113">0</span></span>|<span data-ttu-id="b7e78-114">Значение не настраивается с Intune, не переопределяют настраиваемых пользователем устройства по умолчанию</span><span class="sxs-lookup"><span data-stu-id="b7e78-114">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="b7e78-115">none</span><span class="sxs-lookup"><span data-stu-id="b7e78-115">none</span></span>|<span data-ttu-id="b7e78-116">1</span><span class="sxs-lookup"><span data-stu-id="b7e78-116">1</span></span>|<span data-ttu-id="b7e78-117">Предварительный ключ не кодируются.</span><span class="sxs-lookup"><span data-stu-id="b7e78-117">Preshared key is not encoded.</span></span> <span data-ttu-id="b7e78-118">Вместо этого он будет храниться в формате Юникода</span><span class="sxs-lookup"><span data-stu-id="b7e78-118">Instead, it is kept in its wide-character format</span></span>|
|<span data-ttu-id="b7e78-119">utF8</span><span class="sxs-lookup"><span data-stu-id="b7e78-119">utF8</span></span>|<span data-ttu-id="b7e78-120">2</span><span class="sxs-lookup"><span data-stu-id="b7e78-120">2</span></span>|<span data-ttu-id="b7e78-121">Кодирование предварительный ключ, используя UTF-8</span><span class="sxs-lookup"><span data-stu-id="b7e78-121">Encode the preshared key using UTF-8</span></span>|




