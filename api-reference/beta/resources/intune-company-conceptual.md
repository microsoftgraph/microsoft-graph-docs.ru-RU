---
title: Условия и условия компании в Microsoft Intune - API Graph Microsoft
description: Перечисляет Graph API Microsoft для конечных точек Intune (REST), определяя условия для организации-клиента.
localization_priority: Normal
author: dougeby
ms.prod: intune
ms.openlocfilehash: 59d72416edb38872effd4dcca2a3a898e86bcfb9bf30f131c0ee0b43f8443769
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54170449"
---
# <a name="company-terms-and-conditions-in-microsoft-intune"></a>Корпоративные условия в Microsoft Intune

Пространство имен: microsoft.graph

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Вы можете развернуть условия Intune для групп пользователей, чтобы показать, как регистрация, доступ к рабочим ресурсам и приложение "Корпоративный портал" влияют на устройства и пользователей. Пользователи должны принять условия, чтобы использовать Корпоративный портал для регистрации и доступа к своей рабочей среде.

Можно создать и развернуть несколько политик с различными условиями. Вы также можете создать версии одних условий на разных языках, а затем развернуть их в соответствующих группах.

Для управления корпоративными условиями в Intune используются перечисленные ниже ресурсы Graph.

- [Условия](intune-companyterms-termsandconditions.md)
- [Состояние принятия условий](intune-companyterms-termsandconditionsacceptancestatus.md)
- [Назначение условий](intune-companyterms-termsandconditionsassignment.md)
- [Назначение групп условий](intune-companyterms-termsandconditionsgroupassignment.md)