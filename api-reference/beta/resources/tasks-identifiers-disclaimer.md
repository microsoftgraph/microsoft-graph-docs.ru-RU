---
title: Идентификаторы в задачах
description: 'Идентификаторы объектов в задачах — это строковые значения, создаваемые службой. . Значения: 28 символов, с учетом регистра. Если параметр передается как in, служба выполняет простую проверку формата идентификатора, при неудачной проверке формата вызывающие абоненты получат ошибочный запрос (400) об ошибке, указывающий на эту проблему. Получение этой ошибки указывает на ошибку в вызывающем приложении, например:'
localization_priority: Normal
ms.openlocfilehash: 98a999fa2473a8f77b316d6acf668aec9c3ac832
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32583227"
---
# <a name="identifiers-in-tasks"></a>Идентификаторы в задачах

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Идентификаторы объектов в задачах — это строковые значения, создаваемые службой. . Значения: 28 символов, с учетом регистра. Если параметр передается как in, служба выполняет простую проверку формата идентификатора, при неудачной проверке формата вызывающие абоненты получат ошибочный запрос (400) об ошибке, указывающий на эту проблему. Получение этой ошибки указывает на ошибку в вызывающем приложении, например:

- Вызывающее приложение обработало идентификатор как строку без учета регистра. В задачах идентификаторы чувствительны к регистру.
- Вызывающее приложение усекает идентификатор. Идентификаторы в задачах имеют длину 28 символов.
- Вызывающее приложение попыталось создать значение идентификатора для объекта в задачах. Идентификаторы, созданные клиентами, не принимаются. Все идентификаторы создаются службой при создании объектов.

Эта проверка **не является средством безопасности**. Она предназначена только для информирования приложений об общих проблемах, связанных с идентификатором, в процессе разработки приложения, которое в ином случае трудно определить.
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/tasks-identifiers-disclaimer.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
