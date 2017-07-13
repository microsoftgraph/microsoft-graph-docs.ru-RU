<span data-ttu-id="43d71-p114">Отношения между доменом и другими объектами в каталоге, такими как записи проверки и записи конфигурации служб, предоставляются через свойства навигации. Сведения о таких отношениях можно прочесть, указав соответствующие свойства навигации в запросах.</span><span class="sxs-lookup"><span data-stu-id="43d71-p114">Relationships between a domain and other objects in the directory such as its verification records and service configuration records are exposed through navigation properties. You can read these relationships by targeting these navigation properties in your requests.</span></span>

Отношения между доменом и другими объектами в каталоге, такими как записи проверки и записи конфигурации служб, предоставляются через свойства навигации. Сведения о таких отношениях можно прочесть, указав соответствующие свойства навигации в запросах.

| <span data-ttu-id="43d71-199">Связь</span><span class="sxs-lookup"><span data-stu-id="43d71-199">Relationship</span></span> | <span data-ttu-id="43d71-200">Тип</span><span class="sxs-lookup"><span data-stu-id="43d71-200">Type</span></span> |<span data-ttu-id="43d71-201">Описание</span><span class="sxs-lookup"><span data-stu-id="43d71-201">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="43d71-202">domainNameReferences</span><span class="sxs-lookup"><span data-stu-id="43d71-202">domainNameReferences</span></span>|<span data-ttu-id="43d71-203">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="43d71-203">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="43d71-204">Только для чтения, допускает значение null.</span><span class="sxs-lookup"><span data-stu-id="43d71-204">Read-only, Nullable</span></span>|
|<span data-ttu-id="43d71-205">serviceConfigurationRecords</span><span class="sxs-lookup"><span data-stu-id="43d71-205">serviceConfigurationRecords</span></span>|<span data-ttu-id="43d71-206">Коллекция [domainDnsRecord](domaindnsrecord.md)</span><span class="sxs-lookup"><span data-stu-id="43d71-206">[domainDnsRecord](domaindnsrecord.md) collection</span></span>| <span data-ttu-id="43d71-207">DNS-записи, которые клиент добавляет в файл зоны DNS домена, чтобы использовать домен с Microsoft Online Services.</span><span class="sxs-lookup"><span data-stu-id="43d71-207">DNS records the customer adds to the DNS zone file of the domain before the domain can be used by Microsoft Online services.</span></span><br><span data-ttu-id="43d71-208">Только для чтения, допускает значение null.</span><span class="sxs-lookup"><span data-stu-id="43d71-208">Read-only, Nullable</span></span> |
|<span data-ttu-id="43d71-209">verificationDnsRecords</span><span class="sxs-lookup"><span data-stu-id="43d71-209">verificationDnsRecords</span></span>|<span data-ttu-id="43d71-210">Коллекция [domainDnsRecord](domaindnsrecord.md)</span><span class="sxs-lookup"><span data-stu-id="43d71-210">[domainDnsRecord](domaindnsrecord.md) collection</span></span>| <span data-ttu-id="43d71-211">DNS-записи, которые клиент добавляет в файл зоны DNS домена, чтобы подтвердить право собственности на домен в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="43d71-211">DNS records that the customer adds to the DNS zone file of the domain before the customer can complete domain ownership verification with Azure AD.</span></span><br><span data-ttu-id="43d71-212">Только для чтения, допускает значение null.</span><span class="sxs-lookup"><span data-stu-id="43d71-212">Read-only, Nullable</span></span>|

## <span data-ttu-id="43d71-213">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="43d71-213">JSON representation</span></span>
<a id="json-representation" class="xliff"></a>
<span data-ttu-id="43d71-214">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="43d71-214">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domain"
}-->

```json
{
  "authenticationType": "String",
  "availabilityStatus": "String",
  "id": "String (identifier)",
  "isAdminManaged": true,
  "isDefault": true,
  "isInitial": true,
  "isRoot": true,
  "isVerified": true,
  "state": {"@odata.type": "microsoft.graph.domainState"},
  "supportedServices": ["String"]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "domain resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->