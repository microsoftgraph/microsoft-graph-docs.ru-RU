---
title: тип enum windowsPrivacyDataAccessLevel
description: Определение уровня доступа к определенной категории Windows конфиденциальности.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: c086d0b34e1a58c13468e85e9b0030381b0e8ace66076440d834dbf770a1931a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54253021"
---
# <a name="windowsprivacydataaccesslevel-enum-type"></a>тип enum windowsPrivacyDataAccessLevel

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Определение уровня доступа к определенной категории Windows конфиденциальности.

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|notConfigured|0|Уровень доступа не указан, намерения не указаны. Устройство может вести себя как в UserInControl или ForceAllow. Это может зависеть от доступных данных конфиденциальности, Windows версий и других факторов.|
|forceAllow|1 |Приложениям будет разрешен доступ к указанным данным конфиденциальности.|
|forceDeny|2|Приложениям будет отказано в доступе к указанным данным конфиденциальности.|
|userInControl|3 |Пользователям будет предложено, когда приложения попытаются получить доступ к указанным данным конфиденциальности.|




