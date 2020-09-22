---
title: тип перечисления Фиреваллпрешаредкэйенкодингмесодтипе
description: Возможные значения для Фиреваллпрешаредкэйенкодингмесод
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: e6ad3214eb16e69c6a3da7aa51a69cc8b43eca90
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48056683"
---
# <a name="firewallpresharedkeyencodingmethodtype-enum-type"></a><span data-ttu-id="11262-103">тип перечисления Фиреваллпрешаредкэйенкодингмесодтипе</span><span class="sxs-lookup"><span data-stu-id="11262-103">firewallPreSharedKeyEncodingMethodType enum type</span></span>

<span data-ttu-id="11262-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="11262-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="11262-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="11262-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="11262-106">Возможные значения для Фиреваллпрешаредкэйенкодингмесод</span><span class="sxs-lookup"><span data-stu-id="11262-106">Possible values for firewallPreSharedKeyEncodingMethod</span></span>

## <a name="members"></a><span data-ttu-id="11262-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="11262-107">Members</span></span>
|<span data-ttu-id="11262-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="11262-108">Member</span></span>|<span data-ttu-id="11262-109">Значение</span><span class="sxs-lookup"><span data-stu-id="11262-109">Value</span></span>|<span data-ttu-id="11262-110">Описание</span><span class="sxs-lookup"><span data-stu-id="11262-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="11262-111">девицедефаулт</span><span class="sxs-lookup"><span data-stu-id="11262-111">deviceDefault</span></span>|<span data-ttu-id="11262-112">нуль</span><span class="sxs-lookup"><span data-stu-id="11262-112">0</span></span>|<span data-ttu-id="11262-113">Значение не настроено Intune, не переопределять значение устройства по умолчанию, настроенное пользователем</span><span class="sxs-lookup"><span data-stu-id="11262-113">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="11262-114">Нет</span><span class="sxs-lookup"><span data-stu-id="11262-114">none</span></span>|<span data-ttu-id="11262-115">1 </span><span class="sxs-lookup"><span data-stu-id="11262-115">1</span></span>|<span data-ttu-id="11262-116">Общий ключ не кодируется.</span><span class="sxs-lookup"><span data-stu-id="11262-116">Preshared key is not encoded.</span></span> <span data-ttu-id="11262-117">Вместо этого он хранится в расширенном формате символов</span><span class="sxs-lookup"><span data-stu-id="11262-117">Instead, it is kept in its wide-character format</span></span>|
|<span data-ttu-id="11262-118">utF8</span><span class="sxs-lookup"><span data-stu-id="11262-118">utF8</span></span>|<span data-ttu-id="11262-119">2 </span><span class="sxs-lookup"><span data-stu-id="11262-119">2</span></span>|<span data-ttu-id="11262-120">Кодирование общего ключа с помощью UTF – 8</span><span class="sxs-lookup"><span data-stu-id="11262-120">Encode the preshared key using UTF-8</span></span>|









